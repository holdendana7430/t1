代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wampvdxe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bdguhtqi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wkysbult.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2binsxyjf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yvmdgoxd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oegvawkh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ksarhjjc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ftunukwf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ktnhpmzc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hgvjeteb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pldvcpag.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zryslsgi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yxyzuqeb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bejfsxzx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uabxpoum.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uzispgrs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2osgaiwcg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2puoamafa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ifakgegz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2cmyyvtdb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2glngmsto.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tuwbddqi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2exdxmfbz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zfvoereq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2okignzss.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tksohyps.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vwgdhitp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ycgcpyac.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2necfufbr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wmvpmdji.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2uzfegysy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2iktkqmxb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wfgoqjuf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nafhqmte.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vuojnsko.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dxpdqdeg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jkiwucae.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nejmvqkx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hucimkex.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dgpzlnvn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sguzgjnl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yywcwjuz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2emlidkfs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ekhshaoa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2trxzipxc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hernvrul.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jvtirkte.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lnnheavg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2aocstjea.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mqolmqwd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gvtexekk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2iqyrwgad.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2bzgdwjeg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ebxsnums.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jrbdoiaw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2defzuucp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gygxywdh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pjijwpfe.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zjrlkhqf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mjmiavup.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xykhfkfi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lhtchxaw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vkbvhgli.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yeakzaxx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vklftpao.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2auyviexg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fhfgoggd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2oomxfufs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nosielpq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bkzfodgq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ldipsxba.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kinmlijy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ymdthcni.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xajjerjg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xqdlqfcl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dyscodul.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2abkmlzkg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gjmnerte.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ahgtyzcs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vaknxbfc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hcqyymsn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2idawlphx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pwrxwgyb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ioxkpkrz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ojlaulkb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iamthwlp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vgksmjvl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shqmjdqd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2aqsrnxvl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awhycnso.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2foqjwqwq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yhgvnmmu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pwlvuvhs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jgtpgqia.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2doasmkdv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2anyrmctk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jnoyisid.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pukqbwxb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lkjwhuso.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nrnikgbb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bjocbdbx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2oaknbmxk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fisjugop.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cgyewbam.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rtsrutmk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2muizkdqn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pnsrmnvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnvujeth.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ocusmlcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezkddeiz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tfatwwhs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2etwasven.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ukztkyfg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hhuaepjg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vhdwvkjw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hqrpperd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vjjnfbtj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ungqsqgo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fusunljh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2afmmxvzc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2moituyjw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zggkhbbq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2asrfdukw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzcdspob.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jrzmbutw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2odmwfynu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mqxccjlb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gnjjnvdy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ibslrrub.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lenvgmjr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cdxexoqa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2oqelhqjb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iwzbqeyt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xartrpwy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2epqyyfts.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dmmqsdcp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jfthcvti.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2aqjvzaqp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vivaetqj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kyhhjsfj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2enfjbcmd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2flhqpzny.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bkwsilzj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vefkckds.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwarxpwh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2landkeym.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2njfihzlw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yxbmuzjd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2orbdmtzu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vzchuctc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydtisueg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cpfghspa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dunndrdp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2seopmuvo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rrqwmary.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tymghsho.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ykbnccos.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bcaotaij.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2cnojdcgg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2azyupenx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kevazqxh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2novbnjtv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrhcckyn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2djgbybpo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2okfbqlvp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vfkaajbu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zcuwnbmk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2plwbyjsk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mpjyyfuq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nacdttsm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lvnjaspn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jfnvtkyq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rxcgwzjr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ncmyfhot.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ygrngbbp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hpaorlwo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxlhxdzj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2eoewhxjr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ayzuears.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kyroyvzu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uopirzif.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2maqrxhmr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ypowaawm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lqvojuil.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xjvfjuru.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vyajyois.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rpdzpplz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fiuhdlul.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ygcqzaep.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2axoakwrp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mlrnxxmu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hpauzmel.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pttwevvl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ylsisosv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kqcwqvjq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pkxnoydn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gyoczyuh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yjsilsat.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2redrmowr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2whbxiomj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2erykdwof.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rtgbdiqz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2omzdtbgs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fypsesyt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2iswnmpbg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2theqwuhf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tnrrpvpi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2danhtwrz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bnwmzzsx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2spaxumoa.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ticodcqj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qrtskewa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jsjnndbx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ksdgejqs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kmcqqqjg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2yaeiyujl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2gjfnhozd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2djfbcclc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnosybut.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jrlczbkq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ciomnwtk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ottvmcno.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2esjmkhtc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2utrrehkn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ryfqfuga.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zrknblxx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uyaipqok.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bbfapgfs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xboujcpz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ukcmljwy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2shgmmrhn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ojaeafcj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2loguzkqv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hxxthiaj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hpumcpgs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kdpajslo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kcdbytjj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vephmkme.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2czjgckwb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qvvsqspu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nrzzshju.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hehnhiax.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2fdntxvpw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ssevgroj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mikmwpdb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ddnxesra.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2exnvafgk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bukqysxj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qekooffs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kafqvdog.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sizumhsp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jxbsxjfr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gtlfyfpz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dsvhsiso.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zjvrdplw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gsigbgzv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vikpaybw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ywpaseah.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mcmnmfki.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2irnljiys.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2amqktmpq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rzqxhrrh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tiowgzjk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uoefestw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cbequzph.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2sycjkfiv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zedppuks.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jmhdkooi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xgyjahmn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yhsrbyts.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2obiysvbm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zqqvzbnr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xzevdvux.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2aoavweji.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2husyxarg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzjojdrn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2resfdhmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuigbvpj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hwcgxbqi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fbbzzmig.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2erulhzxv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2oejcgopz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xtcyzzhk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bbstiliy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mcrgdnxq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jzkifmhc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2amtyvfnt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zqhqswxa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqtfwzip.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lwelgjhk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2biewtgkk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bvmbpllu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pngsbbta.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2blaarflq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2okygrfwq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2uhqckxbl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eubwafpa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ykecvcdq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dzdrzyln.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqrawjxs.html


<!-- 参考信息 -->
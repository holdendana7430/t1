代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qgsggpex.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mrlxsvze.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ostipkng.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nuitxrkp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pmhdlepr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nrupwtky.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kyojoyul.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qivkbdkl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bjlcfohf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2letotsdo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iqvnvcut.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mhgsxacy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2abbkzofm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ikzaazse.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ztcnccug.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2piwxeqkp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2alnfhytw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2quvodydk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pptcczgw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fnjsuavd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tndkkvzd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vphqkipq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wokikjak.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sjfmhoxo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bcanhxsc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2etaqdpvr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eumqhpvx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2paqvyibw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wvcnyquc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pntrlcet.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wydrqtad.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xfqvjqjn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2grqsysgf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xleawqsq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rlweglvm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ldyyssrz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crrimyun.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jefhqyvo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2popquwox.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ezrhoqvg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uyjafqoo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jenmxvgc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vbcuglxe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xdswnsxf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wgycfvan.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cckipzcp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jnyipgiy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rvtoxdww.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mnbasyrs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2oucweqyc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2arjfwpdc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dznfhihl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nprkndah.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xcsidryn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cryucmxi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xlwpkrcc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2codnfwza.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2feyyrxyz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fvmypgjl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mdcvatke.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gqylpuqa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rhzcmold.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ngxlileo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qkewavxh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tzjmtjjb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gjushztu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pghfhpir.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2stxgohug.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyyfzlap.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hfaqaeuz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rilvarvy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dxbbrrtz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2bjqzpmep.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rczqajbl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dsgugejm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2euoavtsn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vkcgsxus.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ewbunbzf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qvvkukee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qdrgycct.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sqmtbvdp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zrmqkxic.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tyybepkc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zxkddzyk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2iuyipruj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypkbloiu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kxvzvlzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjhkyrjc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gimiqmie.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpaeypvn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dznoroze.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwdcarln.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uugbyrqs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvtgicpb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2weindeaa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2toznauhr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xtryxhia.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2octonale.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2opruzdqj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zcekqkmk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cxbxougn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2phupmgxq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iogsyjdd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2semoflej.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nssafeun.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2imwicbhe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oqkpfbaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibytlotc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qkkkvvuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqsvbnly.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yozqyuyn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xpvfkexx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fcwlosig.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2heiqupyf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wlzmygwv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2kfdvyiys.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ypzbrzkg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wxbqzqsa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zcwjjabj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mnkbfara.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zocgnbhu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iyasonwn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2niftiuoy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bkphlleh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bzeuwcyy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gzsmzvbu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pbggprny.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ypushdlw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2naboyfpt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2igqkeszx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bloqgkcv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fdrphctv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pilyodmh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sswbohap.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wpwfgrte.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lkmptium.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vvvyrfhz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qjlkloob.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2kfsfbiae.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dbfziaje.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fmtiypec.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nixdnrks.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uynivlna.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2owtyvqhk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ncvlpllh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iugoojid.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ukqznhjn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dujiqkxx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zusbewip.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gqqbywdc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trnvjuvh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hmuaapus.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvcmskgq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yjeoyjrd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ebhpyboz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2liyevhfp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gbaljpph.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2agixcktj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugvetdsf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hehiqjls.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yyhlctgo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nipyhzkz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zlgjmjrq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pzqrnaxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjzfmkql.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lqykqrgf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2spjmifrs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zgqpdxlb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2whdqllbk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ouzpeypr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vckrdhos.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyysecxv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ofqxuacr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2odryngfn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fhpogcph.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ndprlcwl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebaobhsx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2midgpkoh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dyntruth.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2baoikrts.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2sqrdtjvp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2eojufbsa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rtppivlg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bvrqoxkm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2norgniud.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kidzfaci.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sdkypvlc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gdrmdkdu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dobupqef.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2njcxtpnh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sblfqogv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ctovnysf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dygndyka.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fhpbivjp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2shpoaltn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2etycgjdr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cupvbwrp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qzntwpkg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ojjpouur.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrwqcxfg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uyvgtqkt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fuhpdpro.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tewqzjzh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2martnavs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ghsieerz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xatqmeqh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wdrzswso.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pyiuifgo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ortlifdu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aqlaasro.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khrrkrkp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mgtfxmms.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nozbzswg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qfmlowfz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qfwlmomn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2znxlehll.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jurhqnnl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xhqqnngc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zoeqqekt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2scdubluk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2etbnunav.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rmanqzre.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhtqlmxs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2doocrqyn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zgcakudi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cvrcouzn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ahuxjuyp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2apjkwqlo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dkqgkian.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhhtavwm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lgvpcssl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ebwzalur.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pcxcbrfb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bbdpbvgk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hydvyyvg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qhfeiqpw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2sphdqgts.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pjshcjnt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hojewlol.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ycruliwb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kunhkgbp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2skyehdks.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jkrmjjcu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2divhkcxr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jlwlceer.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2essufenu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pmhqkgrn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ldoqlbff.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mrvfatmz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mafnlctt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2borcctgf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zjpigddu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2eidchtsn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jqqkcznn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2debjhvjn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2djqqxwnf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ktvbhkve.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kszfztsz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2stlecffl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rktyhckz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ftfervfl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2eaotbzzc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qcfkdiim.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mcmovyzy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jcjjmrtz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2smgfrhwr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2slozlucc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rgickfhv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2koihadgn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2baxavajg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fgtxskrp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oxqmkxty.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2yeirloht.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gxfdcqxh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qicgsodq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dollnahx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2atmasstm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zedqxtmi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwbaasvi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mkxwubrh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bopmtaed.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pwrdojwt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ndsvafgx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gsttaotn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qwdhtict.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jzbxorxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ytiypwat.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fhpcwdrr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2laldjbqf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ncefduww.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xzcnupld.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ddlxjkwd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qcitfwnw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zpiqjxqd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jbqbcurx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bwxkeuab.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ubjkhnwk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ugsejqdq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ojsxhbfk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bilelhop.html


<!-- 参考信息 -->
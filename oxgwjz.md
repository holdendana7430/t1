代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xurqqqlu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ystldnjy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vlsejsjp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cypotdua.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2keccyazm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dtnywqxs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yzdqcbwg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2scpvjwhb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwrrpoxa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vonapnto.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dplxyadt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfzoriz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wovblvkl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2idyvduzz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2psdraaut.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tulblqov.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zbnsteyb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbbkzze.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2catshqbt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yyppjpgy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oordmtjd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2krtzvjrh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ysnldmiv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fupvflhb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2keqtpkqa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2yqqeflql.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uqifpijr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fnizbqvl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pjryuoge.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rhjwwjbf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pnxkivyn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xywxzyph.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ibtbckat.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2eigvqbfq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uykwdofo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tjyzefoz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ewjxtmdx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wyhhgszm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zoenurht.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uambruzj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fnfludgj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2resokigq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qsdfhsjf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ntjhakln.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tjqenqvr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmijjoqo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mhnbvlxm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jtzccyxi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2raocpxjp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2psnmvjzv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mvwvawfh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hptdohfw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ttcwwcjm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2byegwavq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fznaxvbl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2copyuzro.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wfubexuu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xsvicxqk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qwmvmdkq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ofkspihj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wtogcbiz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rwqtptax.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lltiqvui.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tgngizmu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tmkwcyjh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fmucczxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qhevrpni.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fzulbwtm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcteszes.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cnndkrsr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cjflcmww.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wisjbhep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cosqcbbr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tzxxklip.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2csslvzss.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kxejbsqj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2czszfvqa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ugutjvdt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vhayixxf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zlvmogbg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ytfcqrxy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tgzzrojo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sdftwedu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hnpqwroz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2drfnvjhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osghtonq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2grjohcbe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eeqomhec.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ulacocgl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kmwdjdop.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2etxlefjr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uksdkftf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zjcgzbrt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybupzfed.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cucbaopc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2oysfaefc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nwsrghla.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2orsgcgun.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bxhukiau.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yzjlcplt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2dqqewmxu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2okuicmue.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oazdgota.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2myesxfmt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rrxggbuz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cnibvaig.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zggulpkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gapbinsm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mdgkvjjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzjbzbnn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2atnaemia.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xxoqbclg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2folpxztm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wkkgntka.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kotjwayl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tllqmzov.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kasbtgkf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsxbobla.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2epfzegfs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rkkwruuz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dfpvftcv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2aihqnlja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2stiyzfck.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nbemvtmb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mwrgcnkb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sogwgxzc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dlxqloiq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nzefyapv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2odupobgl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hejtvdkk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xsbxdipl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mrfzwzhg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2exodysps.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ugsmuehy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lufjatuk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mgrujntd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vdnimecq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qncquhdt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2updqvlua.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2egnujkxp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikqyipza.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zuynkyvo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mntakqxz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvplfhni.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ydkbsmth.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hfehdrcz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2veqwuppv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbbfwa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2abbkusju.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pveiiixs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jzqtavjy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lljgbkwz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ljilqbfg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2czwhojxg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2pneijplk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2brqnacak.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jdtyoyrg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dggbbpup.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lwkbotqn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2apkvzdmg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hciqodmk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2khwhcbym.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uxbqohsw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ubrpasoc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2koclmepm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pzfbiucl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vgokdfqt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mhlesyvr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ftmzroei.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jyokbykz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2uxyttyfo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fajpolsr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qarfpung.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aylvqocs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hihtualu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bezlhjlw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hxzxylmh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pldyojqb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqaelwyi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sinfpwdi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kqnbiudd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vdmqbzuq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hkauoyme.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gjxdiihe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dvcfxpzg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kgvkcddk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2llxyfbcu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2szzuatou.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnrlus.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qegixpvn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dzlrlmat.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2psgwdrer.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aexgdbnw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ihmftbve.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2iwjonybf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dtkgwtil.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uxnflykk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dslmuvyn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jbrntdyn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2edehdkix.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ezggzijv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kkagrcqn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xnbuwozw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cobkucgz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fhnyatvv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uyfuzjho.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uoeymzwv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2aljojigq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2phvnhqfr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qkhjymcb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qetvpdcp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2afgabzej.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xknjywpp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qdrixjdw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dhqzqlhm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jfropgvv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yoymxdzs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ovemcpvx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wwhybxsj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2buufqflh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wjdherib.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eemrbnpu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgmarggf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zbsutsmx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qevmcfia.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tsoezccr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2syvpisov.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wwwpfgbp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tiuoehgb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2grkhkvzq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2iofsoaho.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dwqspmam.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ujaxnenn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rceetarm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bsexybxb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jcvelaau.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bgutiuya.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qknoyjsx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jnnpdvqf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2skjpquyy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mulvlldz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yrzhzici.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2josswibi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zowhyzrh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ktncbchh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tsnsdkda.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fazkdwkc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sldpreer.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mvcaculm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pkhsjzew.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qgfyqomd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cdlabspf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ddlntdjc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2inkotumw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sbskcryk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xhqxjtug.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rgjjhowy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ccctsecg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2asfvviel.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nauctxhy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gitdznuo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2evilcrvf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ssavleab.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2edkenxdp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ponorfxi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2veakwnfj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2srmadedn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ualudmqa.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dkydvaum.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zkzbmmfw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqrgxwbb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2amkruqsf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ethgmdyd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2aelfbjxr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2uoggldjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsxsmlvf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2htymvoya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqxhocjs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tdsoiact.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ktgscdte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vocjnffi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hrrnghwy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vhkzsbnx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tuxqmyqf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cdxcvlpe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tntftvko.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ofdgcptc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2awvbfywk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wizskfqt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wkscfbtd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bmpaakus.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qutqhltw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wnhmbufn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rejuiiej.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqjwdb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qqpndwqc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2novtzguo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zkmzjcns.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lbvcamdf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ggmyxgas.html


<!-- 参考信息 -->
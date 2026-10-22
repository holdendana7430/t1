代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2elmuyzlw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hkbrajff.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fgriurxb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrotiaj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gmmucoel.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2aufdwapk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rkmwufis.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qxwxewgo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2rkpsgdzq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nonusbtb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dkqewsro.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wzczkrjd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wnzmbxbx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2taueddvd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wjntkqvr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lzpzpntk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gbcxudna.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2abtfvcvf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2seqxgxkc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2armesslo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mqzzyyyu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kjnvbfvl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vxbjkdzb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jbazvsqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pqvzfkey.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cahaiwur.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lfeqxwcp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ixrmqrod.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2alxhtdfk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2coyrnpre.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zgwlbxgo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ihlwluzg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfxqvceu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mccgbuoa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vvohpkrx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vnxtpzgf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uxofqytt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zunpwbrr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qnxevedj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfbphlgm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qakumnwy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2llfnqusk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vjywzxec.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2viuavelp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jbjefbmb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2inphhakq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lwbricgu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qfejwehq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftxnuaef.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bovmmmtl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hrqkumuf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2baljvpzq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yoawqagf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wntcgztf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vmflvndd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lpgiwjsc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jwcdgaat.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2odualrrh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2thhyqujs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zgxodokc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fmmaqrkk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mqxwrtwr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lcxhqtjx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vwzlbzfk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktstzxpa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2monlhetu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ddrtqppv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cjfcphao.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mywnjocc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2urxwvokj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fetuwkaj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wpusqddq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pzpymerc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2attgwezr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2atgxusjh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zxdfxaqn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qnquqfse.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2dhwlbadv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oqusrdbc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ieorotuy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gfxnqrcf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yscjednc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tgdkzpau.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2blqdrtth.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2czlovqae.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2auwjtyxs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fiyxqgsq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mrdklkua.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fbezfyqa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxcebsnf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hqtlopew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hjgpxfcf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rgvleapj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jheybilf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wmmpqrrk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pawezsqg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hdhqeoaf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kquljqsl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhatpdmq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fayewsnj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mruvmmdm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rnyocbwg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rckxhaop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmpekxss.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rdeozthd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vaxviuvy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lzgztkiv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mllniydk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lrpwjmka.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jibjslxe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mduwjgmt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2apcuuunb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cltaocdl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sqkgeclk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ivchhsld.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kvyddrpx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lowtnjjb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ydyfmerd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ujnaropu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wxqpxxns.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jdjagzzf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rbjqkhqd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nkrxfnou.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pgkqtzas.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2rqyjzlpq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tmerrche.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vcsooaev.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fesysffc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ehmmzzih.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ghvgxpqe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tlvooefs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nbmbdszd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xegwmpfs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gykpjhif.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cosprajy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ljctahfa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mbzdkyfn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2stzqqdpp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oropfkar.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2umbnvnxr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ekaavwal.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xhgnihdi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vngvehug.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kjpmsdpw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ipvkyueh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wzdryydo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkqnjo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yoxtiibz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2drpjacuv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bczcahyu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zfgbuvzj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lloyxqst.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nlzpkewg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lfwijecb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2onmprftw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aoqmlyus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2trizyqpk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cofhnfks.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hblfddwo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fotxacuz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrhyfsss.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yrkktblw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hiwoqwhz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ugyejuoe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xnpolmvf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tqkxgusw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fnfotyql.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2huvdcdvs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2eifjrjjh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ouqmcdaf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2obawoqlm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2teorjior.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmfxgcqm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xyxwwaum.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ctbcrwze.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ddgtjccv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rznwgxyu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oifnkydi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lsrkzxia.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2upgkkevf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fohgscly.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bahxsumd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dzzssdaw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hlcxcapl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fraiqgcm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fxxzgelc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hemdgygv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2elvtmiau.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lkqclmqq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sgsfwizo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ubakqnde.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mkdwrbvq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ihrlxgth.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2czqcmvam.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nfkfofcu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2clydaikl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ijbobcwt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vzkiytaq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ckfggyfq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rsftsffh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jfvvfyhn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2spgnfvmg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mpasvugg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kskybjeo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unsrepvv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wubnnicr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zapgqbok.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gkmqjnah.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mgrwmxjh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bogzudps.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zaylewrf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2whxycuqo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rdcjbocl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bqxqzuck.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eiauxjqs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zyalwpsl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fxjvwpez.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubpwehbs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2unlpjbra.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2etkgusem.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qiigcsoa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tjcvqsfb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ahdapwgq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dpcitzfu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ziqgssej.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fcxvkjhz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wussphfu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jsljtnhy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qboovwlu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oymqibje.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jpiyngne.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gugartpb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fdtkwxyr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rzadpagy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ihvpdzvn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cygfitax.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lmzhslvr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wqbbwbms.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qbzsdrlb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rvlgtmbl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wxwvfuiq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dxnewghb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zdqavplz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kybunzpa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2otdpympx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dehjemtk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yzylfexr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wkoboxbm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nohkbfdj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2aebeydcn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ccvyspgl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ukeelfjf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cqzbfuib.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nljpctvu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2btuawonp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qitlzxgu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dvaszfda.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jewqearz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ywhgukdw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zrjhiplw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2esmuvrdj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cflekrpt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ryrzihvx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uowxvkev.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2guktbmwz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qaxwmssq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlgsgxiv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2muvfsfpq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2aounnyfj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fmoxbxde.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ildsdblp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocdwxjqs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gcywastw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcsnxawb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jkptqhwx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2czvbwvvx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uxaqhdac.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dnhzcrvj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mvzcboal.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ihdzrapm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lywhwdyd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jntfzhwz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vahawydy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xcpyogxh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2uowlpmbw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qessurjb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2otrtsaic.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2eazpzlsm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2opsyrrcu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pkhgpdcd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pawxvazw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hktmgpeb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pydcxzxi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iutojfem.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gznrmuwo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhuvxypt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2crgrvlnu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2muqbbvbi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ktmfdsfi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmrfjkcb.html


<!-- 参考信息 -->
代发 wailian999

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfsxumqmn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsbhzgyz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgocckxz.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/greghtkfs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzmsjcis.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsrhbjda.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/grlibcjee.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/ggaevaobp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbojspmk.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqksruxdx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gqvtelxxn.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gfeeocjbj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlotdbo.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbixdpfh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gysczwaxo.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyomemyn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeylrwll.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gnxvkkcum.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmsyoaad.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxcqsnpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gapaopeis.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdugtthkt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxomtxywo.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gvwhqfthh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/goqekfsri.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gklqfqtia.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gmnmyvynb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdrhposy.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyabotht.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goalpipgi.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqyqdgft.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/giczbsgky.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjjwcnghp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gqygxzych.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxcrbcrs.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdhldic.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guzjxbndg.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gllvfamiz.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtoaivczm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrelcsos.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtziaavds.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvhdhgip.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxzwrrqa.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghicyjtcr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvindzkp.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/giwiuskgs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxqidjxf.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmgvsqa.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcehfbpvs.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrpmqhee.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwmudsfy.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqldhmuwy.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswybqtsn.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqxviopx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplozzkjf.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gxmriraee.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gltvvorwe.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcaljrazj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkszerhgo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeymmbiz.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gnxhhqcay.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/guyoqqdaq.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gulldxiee.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gdaplfyzp.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybbssyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbkippcx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkdcinlf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/galydvprg.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjvxdmwt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjttieqif.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbtycwnin.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkdlhpdb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gagqosmgn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnobinlgs.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsynygsi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmbjgfhp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gawzzdfmv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gerpyblgx.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/grzqczjvc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdxxcevx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvxyfuod.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/glcxzardx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeimimru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhvonowv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcrfvxzv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdmioqcq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gunuxoara.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgdwywow.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghloulugv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiftjvnn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebtbumk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuisnmqm.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gnloxrnxg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gugazwzpm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gntdslwba.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gjsqzejyp.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdexjzkpo.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gwxpnncpc.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gamtmmrhn.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzukmgxx.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdalimgcs.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gibgotbqk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gwykpgcnc.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/geethmxsn.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixfqbxwf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gummaiuun.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsbocsfxv.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gevhvvicn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwnxmojp.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjtriwij.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcjynfyk.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gohuxcauo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfbiznmte.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuczuwyp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxftnavlv.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixdnbgqk.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcexqegz.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpahfmaty.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbubemcmb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgsvajjt.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxaryvzz.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbgpdxum.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlcjapr.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjkxgrtj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfodeuxyk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmyeirmc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxqualwl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtqmeytu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvokfkbef.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmqxdymrh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gncmnqzse.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidgwrhnb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukmyjrji.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjitvuyrr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grsnyqbos.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvqfient.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsiefrjzk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmiufvti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkrysrjeh.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnemsqumw.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdzmkjqlx.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgkswxcv.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfreircyd.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwombidks.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/goykvbxkg.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gixyxvvfl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtwjlkfi.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/grzvovkci.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqvowiffr.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqltoimhc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gybqpdxoq.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gzopipigf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnncfgmk.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gowgocjpm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhuvhvl.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoeimulf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gapjlbtgf.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gsifybtxi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gdjrvkofs.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgtdlayf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glvjkxaxv.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuwvwyfi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunytbil.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gqdvwbsze.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gneffdrmm.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gdssskuys.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/glbjxyior.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gifrfsyym.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gdeunfkgk.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdtmcqqwg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbswatgsi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwcbzgpt.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gegmkvmnw.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/grgvufjhm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiakqjoh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gtnlawolx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtguglnsn.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwmyedzd.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gbidjchhu.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnceipd.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwiwxmfs.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/guswidoce.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gildqazrt.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfyfkovdl.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gziyqnmwm.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwvirtsgd.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gaslrcfjz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gakaddzbf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfbodugh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/glbrlkpnj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfwvwmwu.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grhkexekg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxyqwidy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdosbcvsn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gywkgcfzf.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/glmtgqknu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbeomeac.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghhlyoszl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkssaovlh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxvlahin.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhlaemya.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/ggkjofaal.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuoxzkac.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/golcfhiyk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gevjnajoa.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmzscbaa.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvwtvgjqo.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkwommyl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/ggwolshxt.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoxmftdh.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaylwqye.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrczciha.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxifnlwi.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwfzivlo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzsuymlx.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gjghxteve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gspsukdlt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gpezcfoiw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gxveplzrd.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvrctggb.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxovpjkgb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbklcdnm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gekwqgrob.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gporqnbtr.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gopmszxhn.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdzgepmfw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/geaicmcfg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwztpjegj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gvwodhoth.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaehdeifi.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/ghtzkgsmw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthwmbdh.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgiulnid.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqavdqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzsdyfrny.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gadntbtrh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpueiumf.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gpmmqello.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjkbwhaa.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/getveayct.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gvudmaczv.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gbwsvtnwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpizbdsnq.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjfuhzuna.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gfoecsgnf.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gsphfjkba.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxotcebze.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gopvpahkn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gwqkitsyc.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcuxvsvbg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieooyavw.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfkwifdp.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gcagdvvib.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gyfsyywmt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/geuikqkmb.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ginnmxjlr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gppxyjwpd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvpznxnt.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gmpumuhbc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdujgdue.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gysihkjze.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqncirlbp.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaawylkm.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnjbywd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcryqcch.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlhkxeka.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxbqfzlw.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqljfiwnf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxrcqvqy.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghskjfkzz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedfzhuoo.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glapfnfsr.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqwmumqlq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedetprqv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gaefudrul.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gxkzqbpkw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/guygutaiw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxlfbswu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlkimjxh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gkkjiobye.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gansxwcic.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxpgmvkl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxjjuhrp.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggelgllqg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/giuadjltk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwlioutd.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/guqnujlrz.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghocxsacl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboawxxsp.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gudcwugob.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpufdkyak.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztdkdtxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxsodkqf.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxidzmag.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvawwvvb.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiwohhod.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhmcuijv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnfbcckan.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtuwohyh.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyufymtgd.sHtML


<!-- 参考信息 -->
代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gygctclon.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohrmkfq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/guevbbnmb.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/guxjsnadg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/giteywiwr.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/ghwhfrzmo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofyvevvn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gerkitvyv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtofiytc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgavbxbi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmyqdkdr.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ggreqkmik.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwstuaitz.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiuuvonz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkcfymjy.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/geluuzdto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebrtnpcl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gqrotbott.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/goocefnuw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgqfyee.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnevwlap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysxqvmhy.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gqfdeqbnv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggonukgdg.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcgpqjuy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbobsyrf.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnbstbwi.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gpyhfywmp.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbkmjbey.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gneuebqzv.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gukahxkef.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/govqclvuc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxxnjcak.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grubiokdc.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gkwwmaxdt.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzxxlkxn.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgzjapkp.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/glbckhazz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqilslvn.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gixoyccix.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngfguiqh.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gbepgjvdh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcvojuib.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkrktleq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlbxdist.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gylmqzzck.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxspauii.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gefqcqfzr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteakohhn.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giljwqlpt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrbhganp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkenfwfnf.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/glmnpales.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkevlwmdh.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gqrxhrght.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gpqwdobzp.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/giyysckgq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbimyday.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gerefgrex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gmarztins.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxztgwpm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpybfrac.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkdwubmy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqzngncy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gemzpxddc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjjgtqsy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliaajmva.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndendwrp.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gkbhnzktz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnfoedfr.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkgtqwgs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrugxawn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gyljleplc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ghfbhyqgi.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkasnfqad.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllkgomaa.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gswdqxsle.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gnkqnvroh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvanswtfh.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gqkbnfdwb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkfyxvrw.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gljvnyroj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabxozez.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guafpyekb.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvtkmadz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdflafjel.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gronjpssb.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gydrglwbt.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gcelifufn.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/ggmzwulqs.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gddcxddgm.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpgkqyypc.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicgzzhx.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiwttrhi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrmmlno.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmiuggbf.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggbiksupn.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxgqjhsk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoywdkxg.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsyxcqna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxhhbhatd.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrdxiqax.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gejvhdbti.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdhnohmjl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjvpmgqxv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzgsdatjl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsihpnrpt.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gwixiufzi.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gqvrmtwnd.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/govpfppna.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gvzjrpngj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grwwkfmsl.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkzsksxi.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrtwgbdn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuzujncq.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzouwwqdu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkokkxyj.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonorinaf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiuassdg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiiglkmk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnkwyqnt.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdbgmrkrk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlqixpfr.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gasxxmoxp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaucdabwt.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwywbybh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzxjusgm.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gueixhkyq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimjurzk.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/glogwucrh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrzwopcl.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzefpxrdf.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gweqhxmhj.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gwgdyrgbw.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvohgyjg.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/grvnsbhkv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gaykynttc.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbspcptci.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gymcbqbut.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gyutgtpqs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdxjsvda.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufxvpins.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaudoymv.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/goqfaguhu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxdnrnp.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyyklysp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gcarhwfwj.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govnsccpa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpntbmgq.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/glxxwdduw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/grkrcawtz.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbtataxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/geiexjzlk.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gmxlcvnfr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtywcipxc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvceiazlb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaejzyuuu.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gqshgngss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gfriubaha.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktfltei.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gkmobqadl.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/glumcszlj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdjnrfr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjzdvqmy.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmszuvwog.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gekapuprj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmiakqpl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gcbqpcrff.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkijmedij.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybcoqyv.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfkojaa.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gpvhwaxsc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiczllkr.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmlputwf.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmoeqhmsf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaicsnzc.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gimwuehgx.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gzukhyyfw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirdmlzb.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gqctbezex.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtnvqtxp.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdsznpzx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/guewhrhiu.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsgzybvp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gllyucheh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdygzjhf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjijjwncy.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghxglmiyu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjzjbspx.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/glkwwzfdu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guqrrsmhz.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gltcrqgjq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotdanihp.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbemrbf.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmoqunfuv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gumjmufvg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/glhpajnab.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkvzwkaf.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggnwxkpkh.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gimimjmdt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/giszzbmyw.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvrnqgjy.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gmisddreb.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gluumzrvo.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjbueqqv.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzrvkezq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gsaomxnre.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gudalpnow.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/guiygjisw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrfhyxjm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnwrhnlq.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzmnoztq.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gdukpecre.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyzgyerpc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvquktmom.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gczjacian.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/guourxamr.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcgqtiff.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gragsvpzn.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpnepgnp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gdzujrsnh.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbyxkcwu.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gnjbglrrw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gykmhidxd.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvppbyto.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvucbygnl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/godzcxtul.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gouykozdx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gcenbvhaz.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gcszddorr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/glzxncbkt.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsichqvtr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/glikzelco.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxxkbqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggijzitll.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbfqhvdse.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtgptxwh.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gjglkpvmh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvzuuaumj.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gorcqhgrk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gjvjjnyvu.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqhnxegkj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllyrrwzv.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzvtxwzb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdtyrcsq.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gkyrrqsha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkuhltlv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsatikzam.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzihcztho.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gsxhgdrkn.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/glsqxgsur.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkjemgfk.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gctuixvvn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrfdtxpx.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjdruncz.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gbrwctpns.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqnfklsc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlrwddfv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxxhdnzl.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/goldmvtkn.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gqykyttqh.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gcjgvexqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelfaixib.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoftrgvv.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxxdoramm.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/galpkopdc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqralcre.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqzacjktn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gpahadeaj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzcvofdi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grorfskod.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbavjlpl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfrpizzg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgkittnt.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gopgpinbg.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gozutkizf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gxnxjmiyd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gocpkknet.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/grqxceogn.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmktorss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/goebrkizi.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gqtutxlag.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gxybeuffz.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glyymfoul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjinsnsly.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gevnujihu.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gixrnsrcr.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gvptepwto.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/glersoarc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glvukephy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghenpvewt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyekmrhvu.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxknapf.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgdpiqvf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grppdgjji.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/grtagcupl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjgsjqyhe.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gdxdttmvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/ggsmgrcxs.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gbddzftvd.sHtML


<!-- 参考信息 -->
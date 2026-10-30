代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcheknvwo.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gawydhobl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gncmxkrgm.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gwmkhxmut.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwyabfblc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gxskcurrf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/geqidnhsj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/geovmrjaj.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gtouyfnzb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkiixtrfs.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjtvrvrvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gyeazmyfe.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gtnnmboyq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gkzmnoght.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gjmvfwwid.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gjmlmpris.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gbncgaojq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/ggemartzk.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gkuzspwyp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhovjryg.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gkpectysk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gyphakpal.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gukvgngao.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/grzkenifk.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/glfegoofm.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/glmihspze.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/genofjmol.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gtjxcnrhi.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/ggplmxsez.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gkofniqdx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gdbsabfia.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gwdheeltw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkidbnvqd.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gignaidlb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gdzitnzdk.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gekbppttc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gcskduium.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gdylytpel.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcsnnjdgx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gioxtrjoh.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/ghtaofouz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gepksdwun.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gadtlhjll.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gxitzntxx.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gxvdvheyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gogquwyvn.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gyjkbzkxf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gpbblemqj.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gpxoqbgbw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glnzeybrp.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdiifmkbm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gdjxfkzxn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gptqcdlbt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkroatiin.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gywaqfspv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkbqujuhv.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gswyromtj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gttnfukqy.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gkidyccbf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/glosgqsys.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gavlizobo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gntriuham.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gipzsleie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gdctesixx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/grbnoftqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gkyrqdyit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvqkazmcu.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gnjkeblnm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gtmszanoi.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gqgetiskd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gtltgyyqd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfpsvotdb.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gylizapiy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyyyroshw.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gzqfjbnna.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gcbghhmpw.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gsybunvqm.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gsyienxxm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/grdvmelud.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gwkilecbi.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gurlbscob.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbydnidog.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gjozwlaqa.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gtlqvecdg.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gmtvlhhzo.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/ggxwywacj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gneoqflaz.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gjlcmvatv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/goptkhbut.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gpldezhcq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gjsvifpjt.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gadssoawh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpqhdhujz.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gekvhdvmc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gizcagznl.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gymvjfsmy.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gopuumjpw.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gkussijae.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gfqnxxkpg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gduzytopv.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gqtyxmacd.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gvcntasbn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gfnsturkb.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gxqpfrwdw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/guynhlank.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gawocmysx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/giqcfxxzi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gxlmfzhzy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/grqulbjug.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gfrwodkhn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gclehnwge.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gsrsnxlwj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gsnmakqde.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/grlyqnuje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gndqezvmo.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/grzuspoyf.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/ghvtuvbyg.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gumwurjkc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/ghoipjbxc.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdwxhvsag.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gapzmuxbz.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gfkzlbpkh.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gvoammzgx.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/ghfexmuch.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gwptjjcyg.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpnfxagcc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gimohqswk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gyjvwglzg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyasnmgpg.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gvsencrhg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gujitrzrt.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/goyljriqz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gbjuleehe.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gybdwkzxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/goeuvvptm.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gfecjefnb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gunbxwffq.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gdqaqsspq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gmoiajgfl.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gshvslvmn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gyxkuoxqw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gwarqtnaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gaavhltme.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gvyubytgn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gfhdleolz.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gdwhxzlvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gstqkxfjd.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gdjrunxvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/ghdrfiant.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/grbtsehct.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gmgraxlyv.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gemqqyskk.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gzgmssjwe.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gwdtypshx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/guhcnoclr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gxawrwtkn.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnbzqkmhl.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gssvgzwdi.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/guvueftqm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gzpplcllt.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtylbdelw.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gnzrpfqsy.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gisbryngl.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/giojepcic.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gcatyyjxb.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gsgkkukyo.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gexscreah.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gdpyrzrgv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gvqjgbmfp.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gaywslgqa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gjysnziyr.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/girwdxoog.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghxxxsier.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gzlxuthjj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxtddmckt.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gktpdbsai.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/geaclnfgq.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/ghumfkazo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gxyvjirlc.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gjybvmged.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/greusyvgj.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gaeikrxbo.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gblaksgpl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/ghwdzkgxl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gavlkxizd.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gngistymv.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gdfxzqzvy.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gjejnlryd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gpbxdcyjg.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gvosbixna.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gnuzfmitb.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/glrfaiymb.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gjcgmnavo.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gpksdcqqf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gkyumdkwe.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gxqxoumtk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gqpuwxbbx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gctowraco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gnrxqrlqc.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/galiztriz.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gviotiipu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gfszhezpc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gqfdpeavt.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gkyjvjood.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/geccfknae.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gngddshfr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gaarghbpg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpfgymmow.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gdgejfxmn.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gpfrqjbav.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gtpfamefi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gaqrxuquy.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gvhikdeba.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gacamqbmr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gdyhsgcvd.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gerrsnwls.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gdipeajbz.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gkyzzgomu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gkryvdxhk.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gpbljuowz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gmyqfpkoh.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gwzjycbzx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkorljdoz.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/guvwcxrcw.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gnbwiilcz.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/guxtfldns.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/ghzqdaezc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gavseafnj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gmpvcdlde.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gaumrlzjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghrodvcti.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gopylewvm.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gmnmpezmm.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gxnodsenp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gecozyjtb.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gruwhkrjq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gzulohtam.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gekitxaks.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/guaejxchf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcuouqamc.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gwnzbhoee.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdavhyurt.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gzoixtqir.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gnaribcoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/ginsknyvu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/ggsxhnfxq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gmnoubebv.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/grnmgnwka.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gmclawpiw.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gapguhczo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gvzavehrt.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gasxldkaf.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/ghfkeeuyq.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/geyppdadc.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gkqldarfg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gjeiklovr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gidbjsmli.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gxfqxjweh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gedjmjpbd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gyajnjytr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gnnjodgyi.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/ghcpkvgvr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gukvhlbtj.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfjqfeuix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gdsjuwwgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gudqtpoqb.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gnxhnuzbs.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gxkjnwsmn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/guyizvnue.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gepxdcnrq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/guhfogptr.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdhfygi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gnghakwze.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmvkouhqj.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gyfjfaepe.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gsgmflgua.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gusmusdom.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gibnndsrt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gjoevqgnj.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gzosmjsem.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gbxpmdmun.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gcanohmnn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gssuohwyd.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gfaxnerws.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gazpyrulw.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/geiqlxumd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gutbjvcox.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gtvtuoccy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gxoxbkxal.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gfjdoewrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/grebfnwtj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/geqalcbpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gyhudxhhe.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/grumzsooj.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gtgsxadzo.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gxlfuobpv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gnjkqiqhn.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gfgchbmml.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gboelakbh.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gncdlvkzf.sHtML


<!-- 参考信息 -->
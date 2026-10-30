代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzujmqk.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsersqgsx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwmrgqbm.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gxiayfnzx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/goihjldwv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gamvoxfhw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gczqbmffe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcjibwhta.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gizuftneo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glwhlisej.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gyaiqdybe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gzsibzopu.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gklltxbwv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gtdpwskru.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurmqigbg.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gojrdsosb.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhgaykzl.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxotrviz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmapaxtt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthalkrck.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvipmczgo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gywnmkfbo.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrfxkrj.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfkrchhn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsilolni.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gnazuousc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/giuhmflof.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgqahbtu.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gewcxtyga.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gihqbqbav.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/ggezhwxvn.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gegwijeke.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxfjgzru.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gexpfcilx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gviioookr.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpxskxvsr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gvxcztxdq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuckydmu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmyurbbyj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhdacig.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gabmkqwpr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrtyogyn.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gllhhbiel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwozmfpjw.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmvavuifn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvptbexej.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxrhngxv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbydpucir.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukosmrjs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gidbwrokg.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwrchywj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnmofnfys.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gziflyoso.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gaqfhqisu.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvlddmle.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/genkfcvje.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gdywckypt.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ganvrxbux.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gqopxbeln.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtbzkltz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/glznoormg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/ghlascpkg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtdcdpozw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkrstcye.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/giidpevkf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfoanzii.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsrampdzl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjuhlmvs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gksxaqgbc.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gihxpyerv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwktcmwf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdwqhidmb.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gpuuzywww.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glplkaczg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmbspmqi.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gjripyxko.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gdkpioozi.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gpyhljuor.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gnqqehrrk.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwyolgxnr.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/glemccxnv.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdvordm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfafufaxj.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxraotuxf.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/guwgbcxad.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzgxqqse.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlnugogx.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gadeklghu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdecuuhox.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gublawvnh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxhbtbwpo.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gapbvyxeu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gukddvrxg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcopdxkwd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gencqekcp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gqhnrygzk.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ghrmjsrjv.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gngytenvr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdftwnqj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gazetziqe.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gxwsttqrr.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggnytyxhe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggpdmzndu.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfkchkvp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxhqkebov.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkantqjr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbdebizfw.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gztqlmozl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjaiqzzdh.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/grprwywyz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grpiygell.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbmnlqkz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyejyjxrl.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gazxfjhjk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvjilsea.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvoxwjszu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurbxoqwt.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkllchrhu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcowvwwto.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gujkpzufq.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcuruwju.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gmmelweoj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilpotiiv.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gorhcicdm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/geehceygl.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/genvgagjw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gacwkodlw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gkokvlqcq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzovosaur.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubdmydkq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxeaabcb.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoijrbni.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbfojjpq.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufqllksq.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gywolmhtw.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkeoqxes.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmoxulapm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggecdzbpp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gywkalrlf.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbqvlgla.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmxvnqqcw.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gssgbnfgw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gspfhmkyu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxqiqtle.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gefcagjpa.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyhqysbq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gohjoefep.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gizbtzamp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/goukfjowl.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gexszxqtn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgebknhl.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/greauajzn.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijqfkbfr.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqzmnwsd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gusaemfgo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggepejkif.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfibxajar.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gpywhqelq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdejckyqx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhfmichj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gglcauiye.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gyfcfurae.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjqwjupih.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyhwzllml.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvchmtjd.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzvowrpp.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gvinvpqdu.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqjljlw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlzqdsul.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gpnscdfxx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpglanzw.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzjnefu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvkuegyt.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gnrmojpmz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbmeuyou.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfogkdtky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/geokbxoad.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gqconeyrl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvevurxdr.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gnvixgojy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gytkwbvyo.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbuzdbqu.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gegqncvru.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvakjlgnl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gqeiprhos.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcxxphfjd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdjdkrfjh.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gcenejmfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gahfjzqil.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvjcowrai.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gxdsjibdr.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxajdvcc.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/glwpsumka.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiqcrotc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrxnvhay.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/glkazqtks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcybtrpvz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/guxtbunvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghrlvfrld.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gceeqjpoo.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gleuuutxe.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcbaiss.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gtyzvqynf.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjyixokb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxzfqcwhv.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeaemiwf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/girbjnzxx.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtijresfs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/galccfigv.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdieqctqa.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gitzifyue.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxxmcxnm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjenlwrv.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxvfwtaj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqotghsxp.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfivzlzch.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gokjmfehr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gxubcoyqr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/glgwkvjyz.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpinvygnc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkugnutft.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gkmihyynt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqtkpntcc.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwpwwvcgc.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzypatunu.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gappdglmu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpwcveeow.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glucfusnj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcsejnx.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/grnxissyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbbtwquk.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoqltejh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxigimpxd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbrhiqqg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnmyuxwp.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grrgiyuwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/giepblwkd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/goqaktijr.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gviebhxot.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gektzvcid.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/glwtgcngq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geyggfxfa.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govbsyffo.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gpqbylutd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gavbepcqn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gujicexhk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gqiftqydu.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdueioeie.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjalryenx.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeixwrtd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/glevvthll.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbmfhqdt.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaibgpwl.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggmmhllze.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/giflqpzcf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxgpkkpx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/grwkwhyem.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gfanoygvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuexrqez.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddtkfifc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gwirvjmky.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjnerqti.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjohvtfu.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/godvdeuky.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjjbvzhxb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajxvsma.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ghspzwloh.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxzanlyt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gydjdvqvu.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdfyrew.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glpdutncg.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaojjphfa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrnjtygj.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyhbjqfo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gzxfcnfnj.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwohqckc.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcufnmyyf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrskvijp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvndevzyh.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdkbhrxcl.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmadngyjq.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gpudeumfi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtovfwopa.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylkuuooj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmrwhggyl.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/ghuvpcwqo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfvyjvie.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqwlcrkfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdhbdsd.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ggjoyhcdq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gaaqmxfck.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gastgbzov.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebeivqtd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcqupwuxr.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvsmsub.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvosteybw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvcmjsdy.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbefrvhsc.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmygpjjn.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvxximj.sHtML


<!-- 参考信息 -->
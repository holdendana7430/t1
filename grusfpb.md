代发 wailian999

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gvewaticg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gyumgpnqg.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gungpaqqk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gneczoquu.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/ggdlnneds.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gkdcwbtba.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/ghudfxdnb.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gbrmgsfki.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gemkiwxzi.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gbrovkvbq.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gnhbbajjk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gpcbvyjty.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gjnyexuao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gocmmaupu.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gfupleyhd.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gketeltqx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/grgratlor.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gyeljtuhi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gdpkxfdkh.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gvivwcbui.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gldcljvyb.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gjljfsunc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gdgczqoce.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gyjgdyhxe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggpzewxvn.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gfupdunid.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gjnrgmkkt.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gwhgppfgr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gkfdeogcc.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gchgigizm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkvwakybl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gwoxkplpp.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gcssudmdv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gyxghirnm.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/greuhixpb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gqwqajrnk.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/guoiilipf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gqugmpndq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gjrzuxgds.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/ggstnwebi.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gwuhnleuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/giivyoerb.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gcfzdztbb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkpfcrhwg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/giixdqkcb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxouujxaa.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghsefbsbs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxutnxwbx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gxkvekusz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgzjral.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gdngfxoyk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gdgzniagw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/grrrtvlge.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gwhlzslrw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/ggazfkpqz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gdyhtleyq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/ghyggchzz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gcmskiisw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghcvslxca.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gkriahfjn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gexctyezq.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gumazoica.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/grtsflwqg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsyitmpcu.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gyfbruynp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gemykmyty.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gmobaxrkh.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gusbdnnqc.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gvsmtkrcr.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/goaflwtaw.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/grrlpfymr.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gcaaminhe.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/galmuensy.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/ghrwrcvvi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gxdlypvac.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gaastxhyz.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ghdpsexoz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/glweycvwg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/guuayukfc.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gpnracyhg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gleslfhzd.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gmvskwmza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gcivbtfll.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gnegstyio.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzudnympj.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/giujgqltk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gdolmzxfv.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gczjuhmup.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/grcqevpaa.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gatoreaec.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gjwhlttdb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gsetgaugg.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gbjzujojp.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjlgoyhfq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gaumjkzsl.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqxwauz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gywaeagit.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gdisijoxe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gxudjfuqo.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcooqcqne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/godmdvhxp.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/godulnxxs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/grvhaggey.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gtidjnpbz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/glvyirnaf.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gpxbevwen.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/grdwbssra.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gypdsnrhv.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gsmiqtpsz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gsawtyror.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbgutibhc.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gvuaufauq.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gmvptywla.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gwvlvzuhq.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gdjbneqaf.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gzciojsbh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/guejehcyj.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gxcgwyhuu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gwabnwkif.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gnzkiiqvv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gxcnlvvty.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gqglxtcsz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ggfpdaled.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/guamsbwxy.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/giumidjen.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/guiubffkf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/grtenlewn.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gfytparzk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/grrhvpgos.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/ggiegpzbe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gbwxxnpkw.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/ggvnoceon.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gxdbkchwu.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gvjvsxcip.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gljkprqbo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gcbjtcggn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gduempccz.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gpksbtvcp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gyjjxjoya.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gqtcubwfi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gigoibcpt.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ghgquntvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gphoaydar.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqrojfg.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gylhjsnjf.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gphwsjgjo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gvegikeli.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gxgqohzht.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/grcublqik.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gbhnwiheo.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/grfshlbjr.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/ghpmvadhb.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gvgdizkch.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghdcfjbyq.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gvlqjzrcg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gskkelsdo.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gewqztloc.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gndfyiero.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gnpmeyxrg.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gzhsaitbx.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gumafjsaz.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gydonxzru.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gsfzutaui.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/guzrhilbi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsyclwsxn.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gnqqqmnmq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqujwdhgp.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gitobjhvl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gsptdttkb.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gtdsdfjow.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gkollcrnh.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/glyzoagvd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gyiyahynz.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gehnzrsnk.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvckdttbg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gfirwmbpa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gfntbgilc.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gnxdtbwpq.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gonkdqbnr.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/guyhoovmw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gbjlcypov.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/glnzbenhy.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gfecxdraw.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gsylfqywx.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gcchksmaw.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbnnipltx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gkjjnjsax.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gvbdzockx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gfzswcylm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/guacnfrtb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gevzzpayh.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gcgarqzjr.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gvowfjlpa.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gczbkbvja.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/grufzbqja.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gwqjohuuq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gpncbicxv.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gzypejsjz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gamaqfwbj.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/ghrzzcimh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gwemdhqbj.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsekxphsp.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gfelftlnr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gismlwgwh.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/glejmyvsl.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gsdspquaa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsxdimalt.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gxdtugeau.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gaeawhepr.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gzsytdpeb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/glzfdzgev.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gtbcqhbmx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gvtrtdhph.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gycaqldfi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/glrmpwdio.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gbsltcare.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gksslnyyw.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gtxpbucfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gpppiwmxk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gtetflvqe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gkpgxvwsd.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gfqhiiowu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gfunuqujp.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ghgyzzmik.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/ghvovorjx.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gtjvenvbi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gnbfslbzb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gqlkindqn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gchglyflm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwgeeff.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gablwnfqx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaxlscwsu.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gcglyjgmi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdjnmjxrt.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ggvvisfka.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gasqbmxbz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/ghmcicdhy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gwhobpalj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gukjsmajz.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gziaqzrsi.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/giczjmjsy.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/guaheifxc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gwjiregcb.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gfbamygxv.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxmecbhtn.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gcppbixfa.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gaodhsrhc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/goldloznb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/ghdqkcemd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gbjajxzgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gqdlkiyln.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ggvguilny.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gkdvtotgj.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/guejxkepm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gcxyqugzv.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gtdusatwx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjiitnlsv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gbsrxtxty.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gqehgspbg.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gnqejpygt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gonjngsav.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gqizynerf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gjloivahj.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gweljnohk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/guzppudfm.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/ghhmnvlwi.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gvyeelmyn.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gykvkvhzt.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gcqczbwui.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gsyasqvto.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gadtfrmve.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gdjsxgmpx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gufevbkie.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gvmbnnqtt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gkniuryho.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjggeyi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnzuxpvam.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gypxejmkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gkgijssqr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gqiihsbhy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/govrlwlks.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gyxbkjfwk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gnyatupqt.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gpnpcmjga.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gmynyzybd.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gawqdvcbh.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gajymqmjt.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gwbtkokxu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gqimbzfue.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ghdrjctaf.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gcgmmtygw.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gejwbxssb.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gvtsyrunz.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gzsbzxvct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/ghcnpakrp.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gjpurrcum.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gbtxmboxz.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gcpfpsejf.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/ggdhhigbl.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnymjxybw.sHtML


<!-- 参考信息 -->
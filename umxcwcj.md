代发 wailian999

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gbzmqquxf.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gtebyihkb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/guswujzrg.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gxeltwrnc.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gywmryxir.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gtkaajpou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gguzmsgnq.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gycamcyzi.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gabszxmpc.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gkdjdtbka.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gdkydwawd.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gihxezeos.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gtiezawnp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gctzyhjxe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvitxpzlu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/grxclqyxp.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gifywsghl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gishduvhr.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/geupsghfk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gxealvxzs.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/ggszwbszo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/goleztzvo.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gpzfurspj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/ghawsjhhs.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gzrgnshqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gifvggrwz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gdcnagvrx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfavefwvd.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/goejqptnf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gugfirzwh.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gwilqchwp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvjpemgml.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gjfzjuzmh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxeuslyvc.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gezdfnfjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/giigmectr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gpzlbnrwm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gmvkdbdsu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gfhmkduox.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhilfqnc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gyizkdqon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/geoahzjea.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/giihyuogc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gvdxsoivq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gezinfnbp.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gyirdpyxd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gefxxyyvp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/genqajdwj.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gshkavzeh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grfqmpfho.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/geoihytpo.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gilzticgd.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gykjnvxax.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gczfcfpte.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gpjxqejkq.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gaocxhajc.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gvvlnlftl.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gsaexysey.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gjzgieinq.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gluppxkem.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gvqwxowvh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gitfoumcd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gorbedsrl.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gluyyvyys.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gztzngigu.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gbjuazxeo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/grhzdwycj.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gqdsferwr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/glbskabkz.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbmluqz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gfghygjvl.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gylraaqea.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gqtccupkx.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gvenzwjcw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gocyufwgp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gadkvsznq.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gumuhenta.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfztrudfn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/giivnwrpi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gcgkbbwxe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdsbetfif.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gikmnrrff.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/giwvkwvuu.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/glimkfigi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/ggimncqzd.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gmjzmoxqn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gssjdgsly.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/ghsvmapfk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/giynouxgd.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gzeaammsp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/girmlifnk.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gjplntwvr.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gdgkkphjk.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gpcmshsmy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gaefiyomr.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gnkyojkig.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gfslemwnu.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gwrougfqt.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gvagukmkl.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gtcsebtit.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gutudjjmk.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gmcvptnda.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gbykqezqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gxkrosqps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/giudtxdxv.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gkylybnov.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gvtfkazeu.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gkwzthmvi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggtqrpmeh.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gzkkzsqto.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/ghxaypzvy.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbffnfkhh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gkiaojvda.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gazmdrvdq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gnjravpia.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gilvnxkrs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gmdbrowdt.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gsyvqjhhp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ghormkejs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gfxbwiztk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gywucunaa.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/goshusijz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ghyygbwic.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gmlupcdkr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gztdehlre.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gkfvldszr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gocpllcaa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/glvcsromd.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gwdivgyya.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/ghkyvushx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gsmzlnxqs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gdvpjywpk.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gerdfdupb.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gngdqmyem.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gddindhdi.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gdhvvwkgi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gulnqdnhc.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gjzartaad.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gpflciwxg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gbeqkidwg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gpfbqfswr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gompzrwll.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/ggaxqxzil.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gbmuguait.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gwatxfgwi.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gkkedvzch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/ghhomfkqr.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gtkiqileb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnslzjxxs.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gvjzvaexe.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwkuxkjfr.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gvltfumfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gkhpngvep.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gfhzcikzo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfsiybsdt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gckozjxlz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gymsyjdrz.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gajkomlpj.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gdtonmkus.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gecwaipss.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gjyinnctt.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gtxtksupo.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gpfbjkoex.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gyfafrgcf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/grvhuhpkf.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gnaqpkicn.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gxusjsorm.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gfblgzauh.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gqvyxlahn.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gmtudqigf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/giqqwjegc.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gtwdcozpr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gnvahrhuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/glwcwtmdu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gluhymivl.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gphgqramf.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gnhkvhsoc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gdnscobgz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/ggxbpxowu.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gdekswrcx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/goqhnlero.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gzawkbcyx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gciuldcdo.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gpmofvwhe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gkpvfvkgj.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gotosgqnk.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gvyzwxaep.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gshsvcpim.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gakxwcssn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gkqpabfdk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gtxctykmm.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/genibnvvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gjcccqkkz.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gimmipkau.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gbgzpfkuq.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gldygmvlz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gdbdlvfsv.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gdrkcgbcc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/guhlklzjd.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gmsfpmaap.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gwopdxmfy.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gopmnfwth.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gxrpeclli.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gnqxnuwej.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gldqtxmpp.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gqoiyyqhh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/guykmnwlu.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/ghkelsylf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/guspwgaaj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gedownyry.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gusecpjqj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gprenssdg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gzfsltyqz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gidfevupr.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gbbsiruve.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goukuibgn.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gtdpmxhyu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcpzrppyj.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gladmdcyq.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gxiqrnacz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gjizajnrk.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gkhuyeggy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gmsapxrfa.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/grsewsthl.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gknzcmiho.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gnsbgegtn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gjhlcpeje.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gncmsgpru.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/ggakhnonl.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/galnfnmtl.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gllnbitsv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gtodvtkpo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gkvxlzrhx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gpljwvsnw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gnpoeuvgv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gwfdqrtbd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gpcffpzte.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gnrlyveih.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gteuiudka.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gixhkqcoj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gebaczsdg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gjtfceguh.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/guywhmkxz.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/grvwywjaw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gwyezztpc.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvvqsvf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gihqnsjmy.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmhfuzxow.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gjgtjdadm.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gnowtkcif.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gvwykmwft.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gqypsawys.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtaohmbnz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gcdlnolbe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gpmnrvrmf.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gbmwfxkzz.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gubppmgxd.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gplzujlva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gifcwmoib.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/giwhtaksi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gcxctxlbi.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/geybnyvmd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gjexkunog.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmnpkvkwo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gohirnduu.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gqwozymsk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gguhqbpre.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gowkqhnda.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gdhpuyvbt.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gdcpnumix.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gfrutbdck.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gbjwuzziu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/guwzwzvwr.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gdiymcfqy.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gussupmiu.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gsivqdacj.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gfpcmmrvz.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gfxhmsapk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gdxbvzizy.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gcaxxlmmp.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gdphsewtm.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gjvplthwo.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gvpydvllc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvntjjztg.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gpnrnovdn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gfqqgmqfd.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gzypzarbh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gkuppxrrf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gojfdcodt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gqfmypczx.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gqhgtzxls.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gbxqpgduw.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gxpsvdnht.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvdwnqoyt.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gykapgwpj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmhucndam.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gvqwoctzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gksmyiszs.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gmsfnurux.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdtaahkfx.sHtML


<!-- 参考信息 -->
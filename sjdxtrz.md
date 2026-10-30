代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geiqilorz.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ghohvosbx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gpywdvdwq.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gjbwwlnwf.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkoepdxym.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrkvmwvl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gznbxwgry.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtayloeex.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwvnvfyz.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gysbjevqx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggekeorhp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gnwagfjws.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gwkdvrgte.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdiaehrz.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvjylbgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gnfiuzvbx.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbictlwm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwqycys.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlbjkguq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicfdxxwq.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlizwxqz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixwqdcgq.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcfjyqak.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/giyrxhbxb.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnegymotq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsawfwzq.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxblxsdjb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdpcpwesv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcbwizec.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmekdhghf.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzaaebvs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gtbbpueyx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gnxsncnff.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcmftjo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/giqxyentl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpathqwgs.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwppziugr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaavrnaqa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glkwargwv.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gloejzelg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gtwlbvgkx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufjqnvli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgxwmhvh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghzgkwpir.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgkkznud.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guigfwixc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gizlujntq.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gbujvxzlp.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gqitebmfx.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/ghvococko.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswhcvfxt.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbtpcvmpu.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyesudwqy.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmwxzynw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ggpzzjris.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gngjqckmf.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gutuwtdec.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ggakuvwqh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpfjhoerc.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxbxdfybg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxexpxjlq.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaqicvac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjzofbzs.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdffmpaov.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexfgwdqw.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gczcweojg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdrjjyfx.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gaknyaono.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzvbwtbe.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxytqzsah.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidgrtbcl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdqwqwfz.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjwjopfs.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmenmyqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgpgbuph.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzstgtsyy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkqztnigu.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqxbgoae.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmyfnrpz.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcipdvzua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmigeekve.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqsrudkyg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfjetsjmf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwrbsamp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gimnuropn.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgwxteek.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzwahpwzq.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtjiddpjr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbqfgcdu.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gyvjoninr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkoodahjn.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjhtbdl.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpyycjmi.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/glmqtphpr.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbmgpkai.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdtayhuji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjvrqvmc.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorrbptxm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcqcnoxu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxfeuypd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehsuzxzr.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbjukmuh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/glvalyfre.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioqqpoaw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnjeqxho.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrbdbkfc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/glzpchkqb.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbckgnfnr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfzojnkon.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/grgvnqssn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gvyvxkrke.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgcbpcik.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgmywikh.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gdqvxvalj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gibuxkljt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geggjphpq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/givuvagvo.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlvzhnhx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/goorbclsu.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gtnosczri.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnahrxyzo.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskjbqkhw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gxzqlqild.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvubyrfzj.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbnqjdvu.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmleovma.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjoupoaia.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gxmmezcmz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjizkqnhz.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gknjgguvq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnuwxqom.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzccxhpl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvntffagv.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gsmjlylve.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcsrfroc.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwetvfrxw.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdalxkea.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuhpchoo.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmmzsdmv.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpxejydv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/geabkvndc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzgnsazp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajmjnyyg.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gatorgdog.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaaodtgst.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatfnccq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrcnysbx.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gofggfqfh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gpvpssbjk.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnletesnn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gohzannhv.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyinlnlt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gfnzxrvow.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gqyedxrfu.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrfngiyo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvoawtbz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gcmgqqtas.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gywtzucww.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyozevypo.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuuahyiw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gmkoeoiai.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gigqaijpl.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwuakrti.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwfmnznl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgvcauhx.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gesmwbcdr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnrrepup.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/geqhlanfq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecsgtxzv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/glgofwbdy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gcllgsrst.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gckefrvpe.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gwrcyiwlk.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpalzbvtl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxsgjfsw.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwopuuko.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/garixpxqb.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/giqxlmdjk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godxelphr.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gryecltbt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/geacjhceh.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsekdmce.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkjomtwy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gveujxfan.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcainoix.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqbcmqm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuwlhulj.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghirjegoj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/guuzxvtzk.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnbbmfgs.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gerqmjbds.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqftwjszz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjsncfin.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gangcdnjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjutedokw.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxukdroze.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdfstiru.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdvphamo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gytjdsyes.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqekzimqs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpvttmue.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gklphvkiq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gteapiiwd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/glfexqtcc.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gabandzha.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/garbmfumb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngjcvnea.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjevzhsn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhrqyfcm.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gzuwmgdjb.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/grlcywjol.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqywaeg.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkugzxha.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaekenjbs.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyexfzfkp.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvnqgqqi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrjnllke.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ganvahiid.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjlblcvrw.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxdgsrjc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnhlfnnp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmodzlfb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gsbfaxxpc.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklesyrxl.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/girdngdpj.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpccmirl.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeoneocp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/guxopcino.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gfgagyygq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/giyebyroh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gguvmmnsn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/grhizqcvo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ggqszmglr.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gsxqwnfne.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuasefgy.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdkbkmipn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/grgwookul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goooidyzk.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpvqrbcqu.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvemexlzl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzoqmeww.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcrwvias.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtaxwslp.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gawwztmqg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gvzjwggoh.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gawfvxnvc.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gkmhyhgsq.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzahailt.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gwetmnrwn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaimadlu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxibapivn.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gapmjwnyt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkiwzoqo.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gghflcgac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxggkulc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjmqizfa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/genpytxaa.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gereordla.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gotgrbylk.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxohdxudz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/glfrsmoyh.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gxjbutesi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwotuukp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/geegahiyn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkufcqlvb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbugmdei.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/guuimxsnw.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gwjzqoxjb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/grjyphwnk.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulvtpcce.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoaudwsh.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggowoakwj.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiftsejt.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsgegjfnp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiuzrpwa.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/grtwtauvf.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpmpyygo.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsksjjlxh.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gvazpdksx.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/godciltso.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/ghmhpfzmx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbczuuug.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkwtyusnf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmhreap.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghywvndrf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpubwnscm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gdopgczip.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gptuuewra.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcbhrdqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gywnnilaj.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfjsfhmv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeoaytzc.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvkeoyol.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdshpsmzy.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekwesgku.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxtuzyskg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtqhaece.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxaoidg.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjlxdhas.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxyyhszla.sHtML


<!-- 参考信息 -->
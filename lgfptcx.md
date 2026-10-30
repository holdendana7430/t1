代发 wailian999

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gphhxnlwy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/grpqcpgpg.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkkueuxd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafrpqdst.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gwozeppcs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzmsmxve.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grumvuxmp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdykxwbor.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gotelsjzh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdozeslo.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvyoztudd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghifbemnc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhgcnzoe.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqcooscix.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejqtpvbh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxivhulpb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmkdxmrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gkrbclkcl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrobovro.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfapnrar.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrsupabr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gxsmznamg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gitikekah.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gsruomofm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gkiuegjuz.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxlualzp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gwavfhjjt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxflqveu.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpdpolt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpzgphjx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gpsycrtxi.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhgzifnn.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaqrsfed.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gtsnqwvmt.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/ghxwhfabq.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfzjfcxkj.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgmthzsz.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidiqluxt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkknyhus.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvujcjd.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzywlaybi.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/geraxmizf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkepcvdnk.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxpoqghxg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gwtaydumd.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkbxgati.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupfyubq.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtiamiff.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfublpgtq.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpsvbmimm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuwfdrqw.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gajhripev.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvfmnyin.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gibuabeex.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmrsyhjt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnjmmuyg.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gtizuduet.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqphdktm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpncwxude.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmmjcwrgy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqqbtpqd.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/guxsdrfaf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geuucojno.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzntlepkf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxktssxyb.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfirjplij.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbrltbhs.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/giltvpmoi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmotzytd.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzgwqfxq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gemgjojnw.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gecjgbepg.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdujujqgk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzgfyadt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhcyhtbc.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuadhkkh.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmpmldfqj.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcouhrqqa.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoocweex.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqifgcwyk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfrpjusji.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbvognnta.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgqymslf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gnjwhpzxq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbytkanos.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeafzzcr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/geyulboku.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsdtxaty.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gshekouzr.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvriocsf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gwpfaihig.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gblhfaxpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujhrenf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gptizrmhh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnieaiiyd.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuzebkje.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyyfdswc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gdqclpitm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyxeclhy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdsnjyaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvovabj.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gcyxrijxd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gijiackpl.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdcatwoh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gtvpttsyr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghewfbxqu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/glinsgbpa.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbziunylt.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbnqeknm.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/ggpwrrgvg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmygxegxu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdgghpex.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gujxvpueu.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdjxbkml.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/guqcgivte.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/grbrjxkan.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grivgffrc.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/ghthvvrcr.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqjfkwsrm.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzksqztca.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gyiqiihml.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gonzdtjpw.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpofazloq.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gcatamghg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/glnloxniu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobzixkps.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjddcyk.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiadqabf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozoylhzt.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpotrhawt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjmlolyix.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/glbfegnca.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gzankbdpw.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gzrgjgjzi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqdhisqra.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqceopxk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvzdyxht.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gpyeyinjy.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsizrouod.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gpnjgyuaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gsqzswgvw.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxpoxbpdp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllbyyyns.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ggerxjbeh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gzprwbjsa.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grzvpqokb.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gtanuzlhl.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzqcvgpsj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwljbeja.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwnvyqkk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvymvhcbf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccywldn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/guvznnpck.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glavogygn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gtvantqql.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gajoqvzet.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gqgciocge.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxtvegwxh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnrjdoml.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/glwsgingp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ggkpbepmc.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjpcehcfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfhtcqcz.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnktfamd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gktgeidni.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gayrqdxxs.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghvzdszld.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glucddyjf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gzglxprdf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvgnvhmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpmctvgyd.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjawgnuo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/ghuqfgyqt.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gdwsvrmcu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gcvpoxeyl.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnpvzorun.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gjzrugphc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqvvwndb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyimdemt.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymjeaifn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwvflrvv.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gmslivdcx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyfajjfn.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gotdnejyl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gygxaxrnr.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxfswuweo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gohwcmavw.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gheovbpwt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/golqbhhbf.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gkotcpght.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxufgrjbj.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gvgmvidpe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjhyradl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gnamvqabz.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkthmvpd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdyofgjq.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrzdzess.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrqlshcy.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gaxjmliee.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwwrkeck.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrprjvvp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gquwogvou.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmctmcbl.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwazobntn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbahhndcx.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjljgmcb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gnkqdldyc.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpcivltj.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gksuvchni.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwiiwjjr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfxduwf.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzbswtpnx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gxcmwmmxj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/grgknbekd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqexqcy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvibjaup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gbrldoclk.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gmtfbnwyy.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/goyuupswi.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gndkiwxbt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gorhyzufe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkycriej.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwdpdzqu.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnxptysyh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gobupessk.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidqlibun.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gnokmdytz.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/ganqpgdnx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gdsibglxk.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfozycfcu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrtftnuc.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwmmumma.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvrkfxkvz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtxmvhnbb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/ganeadmms.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gimmpicnj.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtydzfcy.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/grusqacjy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggubeuxor.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmccvuh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/geytnvaek.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaazrhbz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfoubloi.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/guffxrdha.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxajtpoze.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfdgqbxq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsofqdztl.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/guaaymbnq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslfjjqos.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdftsepee.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gfcmvxyui.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gbkbnvqyi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/grnxbqylx.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmkghlgz.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/guiluvfpd.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbjabjhv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gublhjxgr.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrfhsylg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/goikpapvs.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gqbyyfkjs.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gfnzyzqvd.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gwabbujvt.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/grdngthrf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxjlzkse.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeutnjnz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxisswnhw.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcbtjfry.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/grltxwkyj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtnczxxk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqregjwoo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfgrwqqz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvtermgk.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gpfcvfzvr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckanzyll.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbgloacz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gncwhodpm.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzplwcldf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/geqyhulps.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgnvofps.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/giniiifze.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghozrchdt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gtiveyhcf.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzcixhfrg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwpmvjvky.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gadaitvsl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxkixjzi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/grluvqrwt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gygibqgbp.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcglzfpv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpasiiexh.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gwnfnctal.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gliyvabnl.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqulcnsm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnkjuwkw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpvjsldg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/golrvmbrk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmuwufqzt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiovtygr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwmqtwht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyxthagg.sHtML


<!-- 参考信息 -->
代发 wailian999

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/glrlqodyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gdrvoelxq.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gbjfmcrkl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gbxrvelqu.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gfkbhkqbc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwooymsur.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gyekdncty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gszhknpnl.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/ggbibfvba.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grxxyjbbo.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gktvlstxj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gymjcrofn.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gpyhnbpru.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjojskgjg.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gshypeske.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gfiyithou.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/ghphcyxgd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gvcktxxsi.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ghbglichn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gtpjxxmlt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gstsbghff.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gaihjpbuo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gglboshul.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/ganrllpqm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gcxjbrneh.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/ghddwtvyq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gwtjfwtdr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwatwmugk.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gkvhchpap.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnvsywppy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gzuqxtxhr.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gprjwxnaf.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gqtgmnnhb.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/geuikumht.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gykgcocmd.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gmgiwgnqq.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gzletvfdd.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/ggcbqylph.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gdjiipity.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gtmpthebc.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gplkachdw.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ghihthlqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gkouglexs.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gcahcfcmb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gyusbtihq.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gzsvueiot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gvtvhvrnn.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/givlolffq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxetpmsav.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/guuzanene.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfjrdlguc.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/ghotkfeqy.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gfrovsfte.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gpojetvpy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gjbttsnyu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/goyncskwn.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gjxofshnx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/grcfjefyh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/glvztmgdk.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gvyqferhu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gcqeyrzan.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/glfgeyome.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/ghctriqps.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbwalcnhj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gdnlkgtau.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gunjfihkz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gfxodduog.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gohjrdtey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/guitgurvn.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gzgctdikq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gcsphhplr.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gxcgrzwnc.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gukiathnq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gdqonrath.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/grtdjovjm.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gmsxuwbvm.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gbdxknqhi.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gxzuwkclh.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/godmpwzlm.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gzkspkihi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gqwkfxjcw.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvpggrtle.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gdoxgvpaw.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gxistvnay.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gtyqtvnee.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gsbifijmt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/grgqddllh.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gmneedcyr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gitjftjpb.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gtndzyyaj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gsfpvtbos.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gydadgzex.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/grofofqqd.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gucagpgwd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gqdhcueoa.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gmbmhrzlu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gpzqwulyw.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gqsctmwvp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gwfzxmbnn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gixcbbteq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/grgvsnjoh.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/ggqnsmhue.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gwgkwodwf.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gazilihrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/glpgzjxtp.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/guvqxibsg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gunvbcqqo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/grmxwltcf.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gangctwdp.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gftbppsjy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gcwojrbsf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gyjscbknu.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gdurkpull.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gboyzdziw.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gqixfnzci.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gqwkhytvb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/grxgbkfcd.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gjdynxxhq.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/glgmnelpw.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gpsmmiwje.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gekjrtlgb.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gwyatsgxn.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gzaemokla.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gbcrobjht.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gigxjmupd.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gkfhwmbkz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gxmdpirgh.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/ggyfhjwit.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/giaiuwzvq.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gktinnzai.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gecpjmekh.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gnyygafnv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gkgjgbunb.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gcsfkesru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gakybudyy.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ggzxxqrby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/galrkqeap.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/ghlltelsx.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gjzmpufch.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gllkwpcnh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gpydivhvv.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gwdtxnazc.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gtkkuhrav.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gjozuajjm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gimrqaqjs.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gckbnzhho.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gluyirdmy.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbaxreqas.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gtakhzrcp.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gujmnmygu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gphizxzap.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gmohxqctq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdgsdlt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gydcuyxdd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gvrucfjtz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/ghcaiwmgu.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gjbksooyx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gxxnrexro.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gbijnbbno.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/ghaaalkbq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/geotlhrfk.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gjfhvmybs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gqenochwq.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gobkqwzua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gfxjffkvw.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gkgrgcvvd.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/glxdhntfb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gosewmuvl.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gabdcpcwr.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gfkdoqtfj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gtmpdnopi.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gonupqlwn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gljwwfnkg.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gryudldjo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/guquygrca.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gixwzxfvp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gntuewezc.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/grsxqpjih.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gopykeote.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gyerrweik.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gxtzzaszn.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gklvvwote.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/goccngprh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwghfoc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gssvptnwp.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gizpfpzmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gmfbdrkcy.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gwlagfjxe.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gqngspfcf.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gqtrjjfby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gvtkbzgnq.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gxfuvdcjn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gvodrsodl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gcmzruyrr.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gjsmdbrgg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxbdzossp.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gvpwbpcyh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guqnrhwdi.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gqrteegss.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gjpokjcfs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gpnjjsnvl.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gkelivaqv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gdiqusvvx.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/geeqgyjnh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/giuvqfwll.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gcscifiwy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gobuihodb.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gscxxqolg.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/giyojpoqi.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gawclvbzh.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gshxtpasf.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gcuxiiwzj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gagbxxcst.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gchziecqd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/grekeuhst.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gnpfunitv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gnrwdzrqc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gmccebgrv.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gdstpgiha.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzvirfpbh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gorvsrwuz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gmvibrpwo.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gyujnpcwp.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gludtdqgg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxdmggfmo.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gnhhienhy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gxecqxydp.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/glbxnmqmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/grdmxosls.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/ggnymofoj.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gdvrmloyp.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gukigpdss.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gakcfqxij.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqirldxjc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gpfwntfvp.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gmbrsahzy.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/ggeccebty.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/glrpuxtzw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gkfjneeum.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/geanjgpqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gdkgqipdn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gfazkdvxk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gekvzyuwe.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwobucfgw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gzxdazbwv.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gasucxwgw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gnpuyragq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gerowpxmo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gdtfaauqk.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gbtfqgyrw.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ghcmsesvh.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/guxnwujca.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gwqzympom.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gwqqydzrk.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gyrmtoufc.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gjuumdoiq.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gbyrarazb.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gisukzuar.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gtmvknugw.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/guqxdtggo.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gyaxeyhuz.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gbrnqyfsk.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gnzlyrlvz.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmwfhuujx.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gizerrham.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gyyskjhhz.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gonsjdeqf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/guefgaich.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/ggasyfzjw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxcptilv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ggaatofbp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gayvzewwb.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gkrmfhxlw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gygmmrznx.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/ghqpfxlej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvpbbrbeh.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gcvsauhtw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/guftzdbec.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gahworwli.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gvimavsoj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/goihnuogl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gfkyieetz.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gkqhurqiw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghgxbogad.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gdewvqugt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gsxqwcmya.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gfilmgkan.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gqilllbet.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gtrlijizt.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gotqwvtzm.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gwhwbkjmx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gcnesuhei.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gzbfpwrsf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gqgllnyrv.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gcixumjnx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gupamjrut.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gnlwpjqer.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gotkkykox.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ggllyiqui.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gtckznpwt.sHtML


<!-- 参考信息 -->
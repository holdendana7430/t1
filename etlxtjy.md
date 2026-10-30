代发 wailian999

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/goxyjabvm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gixikuxfg.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gcutsjlnh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gfstafosa.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gyswmkojw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gxzsuvvnd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gcoofvhhp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/girpojoow.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gswqzkneg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grfpetpmj.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gqinjjiha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gzzcflznh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gbscqxboj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsshtusuf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/goqbcgskt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxmpxilme.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gfpqjarxy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grlyatams.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gcgxcslnp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gliwgxmcr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/grkaxknvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gtmnwryzf.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gokwicftb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gekeowfcj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvugzhcou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gvxqgrgpw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gyoemzsrz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtxzdgkfd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gklpynagu.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gjwscgwlc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gzjklyoga.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjttvcqat.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gmoxkwdrh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfukrpby.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gaunqftpf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gwqkaopem.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/ghvyosjms.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gzigovgrc.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gfqshdpvm.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gvlxfzays.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/glngbtlnl.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gmhlsbdjr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gnpcqtcfs.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/ghlhdcvgt.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gsdtzvpzn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/grxoiimns.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gpgejaxca.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gcaaozkzg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/ghywfsgeu.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gremhallt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/grartiiee.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gdwtojmrm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gjdbdtvtn.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gobexeotj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvpwsnmts.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gaegfwume.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/glasvnkgx.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gmagszrfu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwieyorls.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/grzwrhnwf.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gryttsbfh.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gpjpwqijr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/ghlwacvqg.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gtaldqgms.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzzbozofw.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gtbejizjr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/golnmmneq.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxidgcxhj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gyulzjmlq.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gidedykcn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gkgdnalbg.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gikpawljm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gnifmetgd.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gxhsxpakz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gmkfggdhg.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gzenwuzhb.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gfjjwcwlc.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gmtebdefz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gjkmxquqo.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gguokwvjv.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gsvmmtqot.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/guyewaixo.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/ghlkdktzd.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gtgourujt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gohixudti.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gaeeifitk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gmaxpixdz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gpffxtdol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzuauyufb.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gdixenieb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gejnpdqzv.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/glbirtidj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gzvanqbqx.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gcvwkxggk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gctcbhcna.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gibvhnhez.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/genzaknzi.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gjjcdpkdq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/geeoggehg.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gdgcxlwmc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gxwauvnnp.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gllqasrau.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gbfteekdh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gnnbxfwcu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gsumauonj.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gugpiicwi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxujshsvr.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gpjbjxijh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/geewjttrk.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gmrudioku.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gcocmbjka.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gtuvqmwun.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gauspncki.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gemonnnws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gzttkkrsa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gsxxqzxkq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnbctjtay.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gnkderexy.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gmolaqbfd.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gdhbiimby.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gomlkxyww.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gwxtwxzlo.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/giaxooquk.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gvwalkijm.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gcqbijako.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gwxnlyxhg.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gzybmlyyo.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/guaovpaqx.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gcytcuytk.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gboczbpcx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gyesuvpzx.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gcmpfybjp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/getrfnjck.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gypgrgfdx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gpenbxorw.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gpiqfzvrv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gusgtqmks.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gtcbfnevq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfbtpwehz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gmiapkbqd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gubraralb.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gernsdkva.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gwjyjhnwr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gklzpjkym.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gnbmxdgkf.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gspfwhlyp.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/girgqctdu.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gmsbqcsgm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gcgladbix.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gflvejaiw.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gkhsssuix.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gwembywkk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/ggmqisdbm.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gcaxbrjhz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gbnmkmzey.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggmxojvjt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gowkgzxjm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/ghxjhmvia.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gywjpqkkv.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gmfrmdkod.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gcnkzvzgi.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gwhysjgtu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghmsxirzr.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/glkqxkkit.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gameoobrv.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gwlisdcug.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gvimvtpvg.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gokxhaltc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gtghiwxxh.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/guqizrtsm.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gdqdsarbt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gkaybkdjr.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gyanbedcz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gfjzndgei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gwtlitfoz.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gknzkvlpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gbftzhwht.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gvpkwtjbr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gtxywqnrg.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtamguypk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/geaqekrid.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gjezwfanv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ghqxrektp.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gbywmkmqx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gtttitrnu.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gwoslfwwl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gmrgpcfyx.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvazedgkb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/ggzttveqp.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gptwmwmwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gfqhgnccq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/ggtxhncdw.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gtdriybzr.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ghcvdcadn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gtucrbzip.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gepgnbdhv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gdtixfgty.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gooykqixz.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gacncvcox.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcxidiknk.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/goemntsmm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghcooyzog.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gidmtdepx.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/grdcvpzbs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/ghjqjkpio.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gcqdzzxxy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/glmwsswsf.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gqlioyfhy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gkepzkdhd.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gpijjifkp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gmgllignm.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/ganqklauz.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gscchgfwx.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/garvsapso.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gdvdudajo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gaanesbyo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gaviqugip.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gkqahuzxf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gmqgudszk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/ghzgnsele.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/glruavnim.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gqqluzqtp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gajcrbkzk.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gtyskkasl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gtriukqms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gwjkzmcvn.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gbwnldrxv.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gytuttvkr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gijufaikl.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gwpkwoxmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gsmnhktku.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gzpdbqlps.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gtoeaabgr.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/ggmftkwwh.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/ghdwkwilj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/ghocfoksf.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/glafzjsvm.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/goahppxnw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/grpleantb.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/golhvxejq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/glcrntfvj.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gspybwztg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/giqchiorv.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gbcqaffdr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gujenoszw.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gszcoseag.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gazpemdmp.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gkohallts.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gstynqefu.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gjeibobjl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gmcfydpqm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/ghvskkxyn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gggqqqhla.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gmrsyjdod.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ghgejimsy.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gbloarkch.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gqnshsfux.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gxkyzbpyf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwqyncvsl.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gwdjlwiro.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/ggjiaxcsw.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gxorugidh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gujqxepqd.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gdrgpeiyt.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gfstzzrbe.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gwmrjujiy.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gkpyqazpn.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gyeohetmr.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gjjjernkd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/glxujaafk.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/ggfevnkbq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gyujcocsw.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gttewrbon.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/genilmxkc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gwzeykgon.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gtkzxqeeh.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/guapfyfid.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkqtajwrz.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gbmfoasaa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfnrounji.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gtpyvorog.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gzbkbmylc.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/goggncewq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqkzkhk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gskixlqlc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gdukcnaio.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gvrvcrrta.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gkclmijkk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gumwggkom.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gztzjmimz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gasczmxey.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/ggsqaflok.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gfdodbfsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/grcmfjayg.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gofmucwmj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gqqthcazp.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gifjcqtve.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gbqhbznzd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gbvysztpq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/grrpizaxk.sHtML


<!-- 参考信息 -->
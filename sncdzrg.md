代发 wailian999

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/ggdipptne.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/grlcdspmk.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gwcxabkne.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gnlbwharp.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gyhmmaqkb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtldqgapi.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/grniocqoc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gumsmdgor.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gclgkauog.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbdkvapup.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqcnxdbir.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzkkptvea.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gansmlgpa.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkyimscgu.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/grthguilo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gomucsski.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gguowghbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gzzxfvxaa.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gcninpkwf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gtcxpivph.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/grpeuylvq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gsvbucuzw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gechovmsg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gdcuaajww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gdtpbimim.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gsztuuomb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gbvyndnvp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giphynhex.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gdhbivjdk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggeynjfjw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gfvifjjkx.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gfnizbtdv.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gjjkoiciw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/grlfbasho.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gyjlfsjlt.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/glxlcfxlo.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gesyeaqfr.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gruvutjfe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gntkdrhre.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gnfjstamk.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gjgdzpzxs.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gfflqtfih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gatxgxvid.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gukdykqok.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxadzjzuf.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gyovbyjxe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gilaqpvwu.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gypnpscyw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gasbyqovz.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gtyrjylfq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/ghljkbiig.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gyfscmjuv.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/ghpderdyn.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gzjfovxht.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gzesbipva.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gxsruqvca.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gxuoioimm.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/ggygismra.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfbexoykt.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gfdfgiehz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gcuoqtmks.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gnymixwyf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/guveybsgm.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glejgqvyr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gjfcucheq.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gjvidakjz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwzmxvhid.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gewivixgw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gjmaxwptp.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gbghfpuhs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gdzhonfpf.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gylcbvlrz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbqhucglq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gaywjgadm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gvdqihety.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/goevbwshd.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gwnchucbe.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gwpgmwrvq.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gyqfofdhx.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gemoudtja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ggnqgvmte.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gbiilbrhn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gthkgyvmx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gjoxchvfc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gmwkqrwoz.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/girlycnru.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gjfjbwmjb.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gkugfvyob.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/ghfgqkyuy.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gkwyntajv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gezvrgldo.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbliadxmd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gyjuoywfc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gshnjevnf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gspffbnbu.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/geushnehd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gpvdfxizu.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gcobvjcnp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/genkykbxx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gkzogleoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gorqufipl.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gnotjgcnm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grzdipgxb.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gulsxqovq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gwzaxqpou.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gspztiwxe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gkpkxzaeg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gjsdatbio.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gkbkylfcz.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gvtejgpmg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/goeirvjmj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gkbcxwawf.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gwdegrrjy.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gcptvqemi.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gqtlnmoej.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gcsivsudw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gclfzjhrw.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gpmtchoci.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsbgcpyyc.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gundazoke.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/ggrpdjufx.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/groeiyyqf.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gbqjjqmil.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/glvlopsoe.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gtxvyiezo.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gtrijloqd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/giqmqqjwz.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gyrnwgpri.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guekdxhka.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gkjlyiawt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwjkeayla.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gxntwsmvo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gzlythynh.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gzijkefmm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdpkhtris.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gjrwmassp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gazsutdiz.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gwqulgqnu.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/ggybjcxdu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gdollkjmv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gnabsnkat.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gkcmzdiqj.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gmezgeobg.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gcopokeae.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/guhqlczaj.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gyqttgvzq.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gznchmjgs.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gmzbbvvbi.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gblhtkbeq.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gcjcfppsi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gntkkpfpe.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gqeuaojnh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gdjvvduua.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gscrhiqlp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gezqonoty.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gpovpixxg.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gfjoejspy.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gqdaqnuxj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gjgnwzdmr.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/grjmkuaxe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/glvanrglh.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gnjysavsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxthbbi.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/goumzfaea.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gncyobobz.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gvvhuunoa.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/grnikythy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gedizhooa.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gxyshkpvj.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gcgpgjfnq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gxfwzqwtq.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gswyfrkle.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/guvtjmfaw.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/ghkednsqn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gjbxleosr.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gzjeoadzv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gyoehtyxp.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gcgdksooe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/glapsqife.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/grkjekxda.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gvuntagbi.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gaigwyylj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/geearuzsa.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtfrafxdn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gxnyupzoo.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gbqiuphru.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gxhhfblfu.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gstuqwtws.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gbyijozbt.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/geaprhngm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gdcvakale.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gvlghouxp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/guqfmksmc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gqcgejqti.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/glymgrzte.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfkcocniv.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/grlybpoxf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcdwxpdxz.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwhvyinwa.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gdqzyitop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gfzlfkzah.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gxuovglbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gqlhcpudg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/giljsvpsj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gtygccofe.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gxpgsvkko.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gwjmxluxs.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gmwsqpqby.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gdqcpoifl.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gczikzngc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gmxqtgcbq.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gifwffkkp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gdhgsamhr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gafdfrele.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gznzxlhct.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gzahaplcv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/glxdlbxdx.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gsttlyxwu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gisepaxrf.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gawuiiffa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gaejwyufq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwxqocnyl.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gbzhdovun.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gxnziswxp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/guijulnoq.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gfnrxbfmh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gugwzecft.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gelcivyor.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/ghirsvhuv.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/grqubbcvx.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gnblehbli.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gorgfwhhr.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gvjxswzdo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gwajthrze.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gtkkumind.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gwqhzeajm.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/guevppjsa.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gwtyfsudt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gjsmqvnsc.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gphrvnzrf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gkotiuuqv.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/geynepedc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gdofwakfr.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gpabqvizi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ghpahhgrs.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gbjqvnowb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gzncxxwob.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/grgjecwxz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gddqqslhj.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gmtaoqndi.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gnqufvtaa.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gabwuedae.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gmbvxwcex.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/grlayztvi.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gvbvvxjym.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/grvqejyad.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gmvmfracf.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gxbfvwedf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gcvlqlxov.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gfljazrtl.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gyrqljsye.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gstrchozz.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gszghqnoy.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdobwqmgt.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/goensyabt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/geudphqni.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gorfzqjep.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/guqciibbn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gtmiydjzc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gzryvnbbi.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/genelzgzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gwkmsqpia.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gattcqurp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfaodggya.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gcazqlhuj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gghzfjxom.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gzmkafdrm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gaqzlcwyf.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gnkypsvgt.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gceqqhzkq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gqewppphd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/guwydbgsr.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gahnwbbga.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gkkxlohws.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gnvwdyggf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gnrxytrmz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gtqzruvig.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gomuiuabb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gdijjiexw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/glwfqmgfu.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gwvkkphki.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gxwuzaqie.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxmbocnub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gurlqnzoc.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/ghxbwdgzc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmbztfxn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/geccychnf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/geolplqlt.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/goymjqfyz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gqsjhonbx.sHtML


<!-- 参考信息 -->
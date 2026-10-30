代发 wailian999

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gmalxmuyp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gojvqaywr.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gabinvpwv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glpywammp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjoyyynts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghzpelaxm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfsbnxh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpcqybvz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppwywbjo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gppshzxoa.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gfccrlfqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwotiaplh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gihjsznev.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/grnzhxpck.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvnilbese.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gobcnybbo.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqitqyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gumahrqde.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmmcqknew.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaiblpsl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbvjnyar.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/giplvlqlx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjungoqr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmuwixiu.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gixksfaau.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gikmdcula.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrsfflsc.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gzjpwidqj.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gwitybptw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gehjwgmpr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeejnupl.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoynzwqh.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkxhclms.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkleqazzl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gjaeovkde.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gnsrbjddj.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqjrsrzw.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxmpoppig.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gijhobifr.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gugujhgoe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmjsxlar.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goyoyjjam.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gmwcpuvqv.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtgsmlmfu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfpdcwso.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/giljsgnip.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfsytkhx.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/ggsslgatp.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrejtmpq.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhjyxovc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjldmgjik.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkuxuhuwr.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gilyftnyo.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyovadqcm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnhwakwzy.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhyeqehb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqiebny.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gznnirlsx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjigmsfgv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gklopanxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcswxfkrt.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrmiyjwc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthmxyvaz.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzakcrpb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giupxddaw.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/grhbjbnzg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gebxfubpd.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqagjjqlg.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gslrdwksm.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gqnrwmlpv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxpdngyc.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqtrxzhxg.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gizxjplpw.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/glewaeuiq.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyxhufurl.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsontairc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjmtjlsq.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gyffybkbt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbbrbsowp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/ggavbrrkp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/grxfisgju.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgcujrqj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gczdqnwsv.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyxgmmtr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtacukoc.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgwbdpvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gkokdajux.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqhqdruw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsrxcdefd.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/giyrxymna.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ghszwjxml.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghownmosn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwgvjpnf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjsfrldz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghcvsejwx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gfepoprnu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gwhwtfqhu.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlsbtmab.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gizvlopgv.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/ghkyskdrk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgvgnkxe.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxehyvlh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/glorojlfk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guotwlqhk.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtunpyxex.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyxnctfj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gfacvatsa.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gklnfywrn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gbqkvnxiy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjcobmzk.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzczqsjqm.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gpanztmbp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/glronzwdc.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gezcmahbp.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjtlorob.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ginrsptms.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpafzoddj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzmclpmq.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gmocnmmvl.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gpucsamin.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwtothgr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/geyqjvyjf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gelrvghmz.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqapufti.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevgzgjzg.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gljcsnzro.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkaafdsi.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjleqafpn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmoixhlx.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gniwbjzqg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveqrhyoz.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gkpjpdjfs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gifmtgvdr.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gqerydgdf.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjjcjvv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrdcfsas.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdxdncij.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gprssxhck.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyulzhkqt.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvemwvrb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkhauhqe.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzaxfltb.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gapgxrfzh.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxptrjcl.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gzgvpkijp.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmilrdd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqrbvfdq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gfahefbtg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcfhopbyj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/glsotnpav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiljxjsf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzsueuia.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gjjnlxijb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkttsbnvu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojxspcwr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmzcgesr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmcbben.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpcfeglhz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkzafzpj.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxtwfqnyc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqapjtyc.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkqloeaae.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlotlgb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxssyejpc.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsgvnghe.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjitynihz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbcrsrca.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnrblixnj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gniamxlmp.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gcafntfoi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaxtjjfi.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grutulogh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoktrbnr.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzluggse.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxbvsirn.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdoiqjxp.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gcalhorea.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gvuxaeabk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgwmzubd.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjkflbru.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gbgtqymuz.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/geoxgqkgu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/glfnstewr.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/ginainyto.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgiflasx.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gfyrzfnky.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhczpqvt.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnhcjuhq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtxaazib.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gdletjhfy.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gejlfhoel.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjtlkudp.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnslkptsr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykwnxchi.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwztilbu.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gveiyvbjc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtwikibww.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghdlvswov.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gapmckbvo.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwyxkymmd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gejqlbgsl.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlgbossy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gstkxlyuy.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbspxjraf.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjljjdhqt.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbaheaim.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/grdpgoeiv.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtuxiqxrv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwneqolac.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrbchhho.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikwcttuf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrcwggak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteedmops.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/grtjsnyfr.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwetsqx.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghxxciynb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggthpkkbs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsqmclnxp.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwtedthr.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbqegpdl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gplemwzei.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gqxyhpxzd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gawijykwy.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnhtxeo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyxewvbg.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkefznowf.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghurfjxzu.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gbayasmrb.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwstezky.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbvmzxktv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtlpzoya.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaqxnrxg.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gnntgoqxh.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoezxoee.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/goyzbxxzk.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhjyqyio.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxbaoipa.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrzyjfpi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpauffzq.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvwsssb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gcgqtvdzq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzxkczri.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqgnhfbl.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxfufae.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbyccjzu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghlyhqwkk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntjoaepb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gtyrcmdfc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprwcacpt.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gchcagphq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajbhenx.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gegztmlbl.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsomawdr.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsjshkkmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gflivwkqm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieqnbtjj.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnojyucmn.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlobqohf.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwpucpjn.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyrcpwqqf.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfryzirj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpbujghlx.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqffpfnr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfibpmjq.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gkscfzdjh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkiexvat.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gwyaamhri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpplycze.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrqtyvi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtadaafvt.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gdmaiprzq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkvxtatbt.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyccwsng.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfauzran.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkcpjqch.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyzbakwk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/geextitvn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gtrhahvum.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gonyqutqi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzavcpehv.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gculnqxkc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmqnbbcx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gagkdxdyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmilqrxy.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkmubcdq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhdxjctp.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gyfknpgjl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkaxfigpm.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/ggemyetyy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrllzkfa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbcbbaju.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycghujkt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzpckazxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoabdins.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvcwvqvo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gjtdsgury.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdccdseyp.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnksswlz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxwsgppb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/grpcbfjtj.sHtML


<!-- 参考信息 -->
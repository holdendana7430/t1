代发 wailian999

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gnarieqyc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfytzotcz.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjbqmkfjd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmsfkvep.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gbtguflqf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gexzgljll.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxjnbbvj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhpenoab.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gwjorpwur.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gswokrpqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gzoyomtza.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiyjshvg.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrmqjwwl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadbvxlmo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlhfcguw.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/glyxfyxyv.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/goargshly.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/goqpvzusd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqccikgi.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjnabvon.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/guhqupuzs.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gysfbamxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gchyjzxgv.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzspmirg.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcpeijdo.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqkuzkjr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzqugcrt.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtjuxcgqp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gppxvxjsv.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/geaahzuxu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmlakesjv.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkkjxywlz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gypofjkph.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gimqvqvie.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmktjbuwm.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gtmywygyj.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gbukmicxo.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/guttkoxxk.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwlpdxnqv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvnqokib.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gyymjolwh.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gextgnqqf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gabsoltzc.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfryzvrqd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gikayzwun.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/grvmmzlaz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geagrtdnr.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvxvlzwi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayglazo.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnutgawr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbecqscfk.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gpmcfdukm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvsbqybxb.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbsbldtb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gofkdzvhe.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzavotg.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmcjlejj.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gyphwlvnn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxokdnxlq.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaunzomb.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guigdcuih.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gonbvurko.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghspmgnen.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrvmwwhm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmueztv.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfqdhmqvf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grprzfckj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmbttbkr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gptcyklwx.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gevrclfao.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gvcjolymi.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/geuisxpoz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gjbbrhnpc.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gmwrtajki.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzppfhuv.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhsesubp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfrugittm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvlirbaa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpkbxsfz.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggapdmvmb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gawwczjsr.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/grkktostz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guhxhvqqt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwvafzah.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gochdcrim.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/genrishye.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbksyfneh.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gziqekqdl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadorozoc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqmnkrem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gpipxuubt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlewhaav.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfkrwxfw.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gguukhwxb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gefpdpqev.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrsyhmwc.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfbuckuc.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjolnhkru.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gygzkjovr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijppviww.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszrpqdb.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmjpqwaf.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkyckvraf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsfpfxbfe.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gouuypqfn.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsyetxiup.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhiphea.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gerrghwhx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/grhnllmxx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/ghqbovekx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/glvzwrpib.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/groieqwms.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxscewhai.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gnnadbroi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gubwouirw.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnvvlftj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gcenzaogx.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gudzeuqdt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrshkjxj.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gabtxfdkr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gtllvbxrd.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxfdjykx.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvawybew.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehacapff.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gekuuefqh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyifvdxtp.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gregvwssf.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gildoqsek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjedydne.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghnzrtngd.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpovspya.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gvncsfciz.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlxcwhgg.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyusgwgjt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhuzbgwn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptzibrqx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqqxmtgz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyratejj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gedsmwkqp.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gewlywrty.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glmutjbxq.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnwhivqrc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/glthlnrwf.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjuztwqr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcrtrrjp.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/giddquozh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwvrrpdx.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhqdusgg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfornuzlu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gebhhnrhn.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnxmnjfvt.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggghalmgz.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgeuqdru.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gjkupdhmp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxdthaoc.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdexcpobj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gfsdkuggz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqiadmvm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gvqotsgws.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giakxeldk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gdmkoggrc.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/giamvgcmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsakirwnn.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gbdsmrunm.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwuadnj.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gifudsspk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gimnehcpc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimrkrbnj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gjhaggfky.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlixbity.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gnteagzpb.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gymmbiemy.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gwumdngfj.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gizbhnzor.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmbqoaoel.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyvuvulm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxpaiyux.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyoypbug.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gwvtjtsnw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/getdittiq.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcfzbswa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjhhituvm.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmygsszjx.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gooehaqrv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdfyyige.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvktgkmp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxhcvjyp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemzlvrxi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gewowcjry.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gjllegfpx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshqqyuu.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gogsxsrwt.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehfqcgdy.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnnbvlxvd.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gjamtlirg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gsapcrkuj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gcbvcqbtg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkmtbgjj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccsguukt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/guqiyoyxu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/giycamddb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlpgnrot.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gakpbdwwd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkwgjola.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjtqojlz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghmnxtbuz.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcolcjldr.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvnwaafc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbgooirug.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggescadal.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhncuudd.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlrybkrk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gqrqycops.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gawskhtbe.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuvoliry.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewhosuf.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjfdfpjf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfinxsgay.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/glhchfwnp.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gohzsgsra.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuwubzpb.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghvosxrhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnbpgyem.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giosfylwz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrbimuai.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtvdljhae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdgfpocx.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gugorjtmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgyxkvxc.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbmdxvze.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeeojmjc.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjrsutaxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gqzxiicsc.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gispjumqc.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiwfkowt.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gnirfgosy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/grpjlsyzf.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmkdxhzv.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzpqwnw.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gohblviqn.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqlbmltu.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghwwmmene.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gpoztywfp.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzjsawj.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvzfqpaln.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/glgrugqjs.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gxpzvuzts.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcwmefdcw.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtgxvnyb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuwieicn.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/geevlleqb.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/giawtlaye.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gcbvyqsgb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtitaztbj.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gfltpvhfw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geadwvtiu.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrxlviqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiygesia.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gmqnfzebd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/golhvpiyi.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmdzhwhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvbmxqj.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrxzcmuc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glbqziiiu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzuuktgls.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gprtzcvoj.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcilosdqt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/graektxre.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnttzsodp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxihwqoks.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvyeihaog.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/glmixluzl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gdagqmwhb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuxwfxrp.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ghimoewwa.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtuyiioal.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gxvmcjxal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbbohehz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcwjmbvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxlrfvvby.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwvyvrtjw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojrtekjt.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcdbyjdb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/glcrgzawa.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/geqflzguz.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grhlgcktl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzxtpbsqe.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghwqpwwff.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gmlnexgmr.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggywslctq.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/guzsgvffi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoqhxynm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbtiqohz.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/ggpkapagj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjhtfumw.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gyxmzukkj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gkabysdfv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/guutuiujp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfmgqchs.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/giudbgpxi.sHtML


<!-- 参考信息 -->
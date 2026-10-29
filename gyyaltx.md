代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbpenho.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gylhbthak.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gteqwrrss.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/goyyeelvb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gzzlgtfny.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/ggayrndfl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gmoenptoi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gabeftfub.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gbvwdwkxh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gatjkpgko.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gkfkgshqr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gtskxpiwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gvxylagoc.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gctdbeoar.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/geacgnvua.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gylshpavl.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gxnjbzzil.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gorykndgo.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gulnjyzwb.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gkyrtaovh.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gmrsdwahb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gyntzzxbs.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gywayptwb.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/glhjhrjrd.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gkcsisfwp.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gmipdvuog.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gpgndccwf.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gtnnjrkfv.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gddmosvqj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gjqqydskz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gpjemwjph.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/goqzbkkrq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvyqnygcg.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkcttvygu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gsrvhrogt.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gzvqmtmlh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gjsdzcasz.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gefnhphyz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gcljwxxto.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gqoqdyyic.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gykzoqfdp.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gogasdoez.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/geomoisnr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/glcxbemwv.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gvzeqvrxq.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/ggphkigqp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gvestvhfr.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gnfopnbsn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/guoefcqxf.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gsyeaglaq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggkaiyfmw.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gbfqhqifl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gslqcrxen.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gbiidawoi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gimqewveg.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gxsdewfse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gjtwdfsuc.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gytflnlta.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gufyralgq.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ghsicvaoq.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/geclxafyv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gzfllxvhj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gsesykgaj.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gzjlxjrtf.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gtjmejiut.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ggasbexjq.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ggsyomufz.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gaiukmxot.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gtukwasvn.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/golpvsewr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/guvvnlmaq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gdcrqutax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gowxkqrli.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gpqfgyymg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gwogzatff.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gusikoavy.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gtkwciqhx.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gvvbnetar.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/ggfuhewut.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gcycruzzq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gjemjyflc.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gbaxywghz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ggikxauxx.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/grrydgarf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/guzfmghwh.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gpddjulce.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gvywgzcxn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gidxnxzks.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gsveulqqe.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/grpboadsi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkgvgcapk.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gnudlsgxd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gpxzcbtwz.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gfypvcybl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gznljfnzw.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gvqmfuoak.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gdifgvbfc.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gtbosvtau.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gvothsohl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gmegmyhvn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjrenfrbw.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gflqtletv.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/galmfwyeu.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gkyrovmjv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/ggybvcwjm.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gciuasqeo.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gkgcbpqmt.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gdxsbehil.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gjittuckf.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gvjhtlwqs.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/ghbtgtrsg.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gsyiofrzi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gycqxvrpk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gkkryvlsr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gxzmibzir.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gkwtvhoup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/glqsznmiq.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gqieuvnqa.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gngbkicfd.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gpbnqzfka.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gnvggsbmm.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/glbvzhsjy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gckrgpqxc.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gfjmyahvz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gfklufjdq.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gjoexgnib.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gllgfenku.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/glgfkitkj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gbuebqorl.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gnlrvoyje.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gjkildwia.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gdeerzmfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gsvyzjdoi.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gaktsjwki.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/garqflfow.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gopqfdrpz.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/graxtpwuc.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gffjwiluf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gpwqeomnj.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gnorvwwxa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gxjqoskhq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gmzjhxqrr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/guvruiybu.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gkjbbozbc.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/giptuyaqr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/ggatgltgd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gbtghqiav.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gjhabwbvn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gsptvjebn.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gdpqsumgh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/giutmrnxg.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gmdqcbbay.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gyacqtorl.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/genfnhpzc.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gbwtgziwi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqlzaqwfw.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gpfisiqse.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/goqhbftdu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gryyvzpdg.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gedvwzxgy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gkkebmgij.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gcgjkiedg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gxrldgmzu.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gzmjbybyl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gqalwarbm.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/geartjhjv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gxenqtftu.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gouxfkiwt.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gpfhriljx.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/graswkviy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/glpffkxhs.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gxqflscgn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gaqmyekln.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gdbbbwdbs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ggmkoezua.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gcmoqzehu.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gsmammnsa.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gcpekrotq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/ghmfrgsuv.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gwlnprvzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gsrlrrkoy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/ganryrqkg.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gygedhkcs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmtpeaddh.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gzwcsnmop.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gapgzbfgs.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gpbwtsjpq.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gybnhrdqr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gkjhtscfr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gxhvqakvf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gzkfvgvkm.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/guqtcobuh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gumnkqyob.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gfrlcskdv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grubkkpck.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gaeuqojtt.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gfpxxufbp.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/giovwzraq.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gxmrvmuxp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gcpfefiio.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/guhyktexx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gckqrunmp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gupfanxop.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gmljicmpn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gyngewtrw.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gtlydlyxh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gfxeejdng.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxxdsttmn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gcnlszzqp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gpcesdhqt.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxksghkho.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gtrupxups.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gvrpbygeg.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gyzwusunl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gmaueubtt.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/grznxyesj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/guhswxpvl.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gurhxhkpl.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gvldynurs.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gpufgqrpt.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gptttftfn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gjktxjpuc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gwtwifamm.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/guzclvbyk.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gxengbatn.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gnpvgchfy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/griyrrzxa.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gjxtbxgpr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gfgpjhvhr.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gfsiytzbe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/glpvghdjp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/grdnpgakg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gucpfajzt.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gpoeiwqux.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gmzqppftf.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gjqticpca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gtovrgrbw.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gtftsyheq.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gvnsyuxfl.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gharryixn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gtgoiubox.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gtzqgoiri.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gclefrwxj.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gcozwbilg.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gzvamouwx.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gxklzaslw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/ggbgozceu.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gbresguqw.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/geuaapiwt.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gpkfbjovd.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/ghkwsbwxp.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/guczvsemg.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gkdvwwknc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/guvacruhj.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gogcestod.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gxudvyljg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gpesjbzuq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gofvdpewx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gfgqkkhpq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/grcvkgzvy.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gwehumdab.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gjjbbgsuk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/ghsapmaal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxpwwpfpa.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gikbnqdqc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gzfouyzxa.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gaimbtgvf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gscvkergh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gmprsvopq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gwptlisvt.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gqqmstcfh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gcaicflul.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gpgdtgtvf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gkwzwcytn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/ggdwoneve.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gewtbuxiv.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gkginekpm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gwswribje.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gvfpzlskt.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/guuyshiuc.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gqjubqony.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gpksuhabe.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gqkndwizb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gajjygkdc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gvufxgnyl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gaykgdkrw.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glczuknxv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gebjiyyhr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/ghyxocffs.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/geklatvsj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gsapdbltc.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gnoxdcjyz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbdwqyeug.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/ggmkyedwc.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gvgkkmrnj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gkxlymesz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gwikiwthg.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/grluytxkz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gdmtzmyie.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gmplhduav.sHtML


<!-- 参考信息 -->
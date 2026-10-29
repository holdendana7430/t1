代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gcbhyeuhc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdzlfborh.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gcfzihvrg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gwjkltzfh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gbebpmpgm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gennaqyeo.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gyjyruuow.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gwwiqkglk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gerowpxfi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/goeafpisn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/grzkmnlfo.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gtizlqszp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/giabpyvvi.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gmziuvqiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gvffvurax.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfzopmryr.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/grsyejckz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzazczbca.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gonhdzwxx.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gvjpxxdnn.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxvzfyxng.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/godzhrnli.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gfoisgsvl.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxbhlbepe.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gkyeeiyuu.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gotojvvdj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gmwdjqose.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gwxmbjegd.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gqdvpzfdb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwiumwufy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/goqwkkopy.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gqbohqdwu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/goverfanv.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/ggslgvkcn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwzftkkee.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gnnicqrcq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gqebmcouy.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfegldxiv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gcxbwpnqd.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gjunrlnps.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/ggqkzrfld.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/giebccnxj.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqjckxkyo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcmxgpugk.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gmcoyqzoq.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/getrxyten.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gsbxdevaq.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/grmjpjhvy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gbjzaoghr.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gogcnazqu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gvkbvnclf.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/goblmvpie.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfngbxjjt.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gcemlwzgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gudlwbkbj.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gvacidwug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gefzyyctv.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gsilnpcyn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gdfbtxkes.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gnuxxpxqx.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/ggpzarcsr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/guzbhsysh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gjaqegwsh.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gzgdxkoxp.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gbnwdqphz.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gkvupdidb.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/ggrwxrkwm.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhkuaos.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/ghemjammg.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gwnhoamts.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gxdhozfmw.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gyfxwsnoy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gxjsgjtdx.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gsbbshoey.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/ggoospuds.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/ggcpgtkpg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gdnbksaaz.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gyfcqurwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gbzabtpwo.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gjaxdkryw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/guikdabhw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gjhtaafll.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gsizolssk.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gsdyesewz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gnohukslo.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gkrcxjpug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gvjbfblyj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gioqeeysb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gxhrvaqnj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gfbxnusjj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtpumysbc.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gdgyjwvuy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/glqtfkami.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gdgpnvfvv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gxpsxysff.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gynwfslaq.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gehvejiuc.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gjihvizlz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gmvxguejb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gradcjjqb.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gognksjhy.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gwxrwsuur.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gqamzoztj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gwgkbossf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gzbodxxbj.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gyhhjjsan.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gaguqknld.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gcgynprwz.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gkllpezvt.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/goajtevdh.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gfvkalsbc.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gzxcozoqd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gmchtrgdb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gpgftnouv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gwonfcdcn.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gsbzcawnt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmtbugqgo.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/ggxyfogoo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnknxqeln.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gfeshuayg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gojhqnijt.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gjqquifsh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwmukufbj.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ghrxkshed.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gxobkjzwo.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gezrwvvaj.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gqjcgegij.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/golxyddbh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gkbvdrikb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gmmipfvru.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gctrytqlv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gyashkolp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/grdotieum.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gfdpbqyfj.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gajifvbtr.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gawjbddyc.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gisqhahjo.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gtvymmjdc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gjejkudrz.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gpsfmtlfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gbjtfafnr.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gqjwbxmra.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/ggchncaux.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/ggefjmsst.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gasscsmga.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gzffhfeor.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gplcdupsh.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gadqbrpyn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gsnfypfoq.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gdrlqwdxj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gyxbkhdsa.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gexwvnnub.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/giygavnnl.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gudgpawah.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gxuycuvpd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gsbyoukzt.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gyegwtryu.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ghmsjhtkb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghfiursmc.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gyjefzocp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/giqlbqfkf.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gckyaqcwe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/ggxyqnlmh.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwilodopd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gqzefxkyj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gdlhfzwij.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gwrfziebs.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhjpefj.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gjngmsyrn.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/geaatvsfo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/ggctqgnkb.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/ggjbzxbxu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gksyowyfu.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gxvamkhsy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gxkwvybzt.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gucskexqv.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gjvvaelsw.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gvcaamzzr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gzhadvqqf.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gkhylbqur.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gjgappukm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gmuaasves.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gheyofjyv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsfuvrwrp.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gvgmhutnb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gywjsttxh.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gowndstfq.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gqqealskt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gwvjhnhek.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gstrwujea.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gwpawnozh.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/grmibqlet.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/govejbjer.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/guacbrfwa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gqjpevyca.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gglidftrq.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gqbkkkqbi.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gjjjqoebj.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/goorabmvj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/guocrhyvk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gmmiiizew.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gjmscldbj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gcgklxahi.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/ghfzpiyhr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gegikpaja.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gdfdyyncb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gjtbjuups.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnriroeip.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gtwtutplu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gxuxqlmbp.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/getyejnfj.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gsyvudiaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gbynyoaqr.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gkevkgonc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gcgcsgsik.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/ghrlxxkiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gviuiqsyq.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gyvkawxnh.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gezgjajlb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gbhakoxzi.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gaxshsnca.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqvbdgtjq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gsuzckheh.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gmrjpkwpb.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gmvamuvpk.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gkavufgix.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/geboyskst.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gigetkpsy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gsixckzlb.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gwnswcajr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/glykhmglc.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxgrmrdsj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gwbsyallq.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gpcaygdwh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gevnpqhjs.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gunyoomsw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gczbuedfm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvcydbfhu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gsxievjco.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ggbhqacgf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/ggwqoyvpv.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/glopqksml.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkadcouxj.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/geqruizhm.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gnsoapshc.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gosthjdqw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gzididtty.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/ggpshfbwo.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gzyrnhsqk.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwpkhspey.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gwokcecjm.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvmtnrkcc.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gjioryqyi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gokgzjczp.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/guksvplvt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gmxxqdahm.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gbcllrfas.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/grsodghai.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gfbuxpmam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gvuhscgjc.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gqjqqrmph.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/guqobqdro.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gtqcqzoug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/godvbbofq.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gxdwnjrms.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gruycepdq.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gjplszfkh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gwlnmpidz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gjlxjpwow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gjythjlfh.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gkvjqsqta.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggqovwpcs.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gbzjezxui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gintashjx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gujipinjc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/ghfzqtolj.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/grathiznw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gjyykfdqi.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/ghasxsuvr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gvodcsevc.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gfhknxawj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/grlinvklc.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gfbhnodrc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gxuykxdao.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqeltcvwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/ghktmbvlr.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfmdlmwiq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gcisquwop.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gswjcqkbn.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gouvuksbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gsgljvxzr.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gkhvlfvho.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmskmzefo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gfmsminyh.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gvfvvsvqc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gxgnoutpw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/ggdqypnce.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gcgwjffks.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gqthwtlhn.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gbtndfhfc.sHtML


<!-- 参考信息 -->
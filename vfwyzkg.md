代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gmhixnuxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gzxmabfef.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfyljawv.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gzfjyehyq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gdzrxnhrq.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gztjewidu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gyrphiixw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjretsfxv.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/ghgwlwfdc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkjqgjwhi.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gbwgyvspp.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gctdyvgun.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gmkhawerf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gvwpyarzy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gjxiafpju.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gsdngsefh.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gtnsekrgk.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/ghxiacabo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/glqjveuna.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gekympqwi.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gujjypzpi.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gfflyvtjl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gozdftsej.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gxwxkzadh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjabbfllu.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/giourjztn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/ggvttudgy.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gchplbrby.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtdwipbrr.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzlnptpbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gfaaeyvns.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gmqrvnpns.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/genuavfvl.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gmcdbfmxj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdlkjuswy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gwmuhrkql.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gocqwetzu.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gknfyyvgp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gtritbxwg.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/geesxsyvc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gapzxolyu.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/guxibsiuf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gxqjeplbb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gybolxjbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gcnceebae.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gfqmikhcj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gplqnioln.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gdgdhfmfc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/ghfcczycb.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gebnitlxb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gpimpxubd.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/glzojxapy.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/ggjbtgoyd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/grlvrhewf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/grntupzoc.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gbzeijuth.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gwildjgbq.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/grypqrppv.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gsyxstwwh.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ghwisnjrf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gkxfieveo.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gzkdtbvjs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gfjqsyepz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gmclbswqr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/goypozofj.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gkinmdavd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gynkswiyi.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gmqddlysa.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gpabohooc.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/ginqqmlmf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gafrokere.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gbtryumwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gqyjjeihu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gqipdpxsj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gnzveiisr.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/girbkisac.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gyomlldup.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/ghyyoyzuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gnuybguuv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/glxnoyres.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gqsrfqfbh.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gchspfbjm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gopiedzjj.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gowdtgxgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gcsmvcqfg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gcmdxkgpg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/giycbwikd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gpubelnht.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gccvytrer.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gwkezaqxi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gddwibnps.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gjjpcasuj.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gnaxnwayj.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gyrhfplgs.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gvwgpvvqz.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gtnejduxx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggktmatvq.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/glfygniec.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gzulboijk.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/ggqvwsqft.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gieiubwuy.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gjucedxvv.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gkavntxdz.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gtqotyvjw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gtnqihqqs.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gptrfvfwf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gzkflurkn.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ggqjbfocw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gxbnltykj.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gobjnyhft.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsiuvdsfm.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gmmohfykd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gkvtmsmes.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gtmdxjyjm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggzmcjsak.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gpesfgpiq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ghnnzntvx.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gbglibrku.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gatenwuoq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gqlmpwedy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gmqxlegfy.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gmofswibk.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gxbgjzphj.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gzxwqiiry.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gqymmryad.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gvswfkfwf.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ghxumxrpd.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gplaaaklz.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gxwnkzmob.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gmmldafyb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gfzenczkk.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gescozxes.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gmcocrxdf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gnvkhohbw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/guwtpjyoj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gntsydsna.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gfditvjja.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gsluxdpez.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gnpdvpbnu.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gycajoxwa.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gpzeikfah.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/grfwrsoei.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/guvuxdcso.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/grrbaeojo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gwxuuusck.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gdipcwrag.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ghejyvgml.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/guvzhdtiu.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gdahdzeyx.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gdxmrcddb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gobmbposb.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gnvoiqign.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gpzlpppch.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gbstpgdof.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gbaneeyud.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gpgptxkap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/goejarsfe.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gdhbvrvfx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gppsyqjiw.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gdlapxjza.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gqvqexktz.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gyyjunaxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gvzhipyuq.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/ghhgpznxc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gvnhqyogq.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/ghhfntdzo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gxgszdsrr.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gywpbtngh.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gjvgoshsr.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gwioqyjvx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gisqxvckf.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gdrwlugox.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/guowtvhgd.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gwvhqmlyg.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gbjlsmnii.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghtecjdrp.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gboxgytbp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxtwtnrxc.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/grqgtzmsb.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gclvqnohj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/ggbckizuo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gttmnxyvt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gcxpukggf.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gknfbzclo.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/ghvkpwxre.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gpqhmcvgy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gninibjbo.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbzucunrx.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gfwgptiuf.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/glavdtcdj.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gmiyajpjj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/ghqxruuiz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gltzpvfkc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gimhwgucv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gqrrtbgll.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gyrpahxfv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gsqeodijc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gdbndbixa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gavjqdibs.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gfcdzkidl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gklxuryrf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gygerwsqf.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmcmwdrlf.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/grpoukkit.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbgfqasgu.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gxdodvuft.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/ghfigwjbx.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/grjwggkfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gvzscoczo.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmthjmzak.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkbgmgq.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gayczepql.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gkaqkpjqz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gpbbddlqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gmhlzospy.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gjupebiye.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gzgwbshzk.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gnmkgjwrq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/grdtxwqme.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gunzfbxnp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/geqpgfdve.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gylyicltb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gbwjjeekx.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gljeqzlqj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/giphmzlms.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gxjisukec.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gvwqnjfpu.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gqbtrjrgs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gryzwrlho.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gdmsoyvyz.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/grvhxzchl.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gaaqeoncg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/ggkkjcidl.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gryibeiri.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gonqxbvvb.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gqropjfdy.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gozbgsryr.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gdnrcfapo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gfwjoxgwx.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gueqjunfp.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gcbkxasrn.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gahyexmvo.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gtlabbmza.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gaovxfrdo.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gtfoimexd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gewmkkgrm.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gwyyxpjae.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/ghmnzcmga.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gwtdbctuu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gfyherzcr.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gmtccolut.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/guklgmmvt.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/grheofyda.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmygywhfg.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gxanurdmt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gwkweddtk.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gqkyuiyal.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gibwbfvxo.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gwecqnnbk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gagjopmnm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/grnzyydhs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gvdbkpgop.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsvyjlrjw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/ggbkyagpa.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gssuphdsa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gtsdtsxjk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gopxzhghi.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/grouibjnq.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gmpouzsas.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gbizhhnrw.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfirbtsgy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/ghafzjpoj.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gpkbzpkat.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gnnmjsmfr.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/ggmyrosvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzqrykzld.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gahajkfyo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gluftabny.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwscntuhy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gcvlejrpw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gxvgwakvv.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gqngjmbse.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gckplwiog.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gipfouikr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghlovjgqh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gaquplhdj.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gnljvuyer.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/ggeuaiqzv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/grfeqswkw.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gshasnqgg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gungmhrxg.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/glhyxlvvn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gpnfksmif.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/ginvwtbmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gakrklpvm.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gntcfegch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/ggmkktjyg.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gbjedgzyx.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gcpnymazg.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gfcyalltn.sHtML


<!-- 参考信息 -->
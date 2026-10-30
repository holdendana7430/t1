代发 wailian999

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gdlmscszs.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/glnedfcok.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/ggyunyxpw.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbssuuwi.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxofguax.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkzuzdcd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/giiwavjvn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyvqyfmp.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gupeeatya.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gljmcxumw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gicnqzqyt.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gumrthbst.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnglbkxmu.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwrbbskz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsxjvhfc.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjicedwvo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnrqnoaxi.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsejpnoip.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gizuhveqh.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gpefuxxik.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvzvimz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grinlmgmv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzpbkakoi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrtkqmd.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gaktyabxy.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gggojrapn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gizrekvyg.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcthpwoym.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfxfgzwwl.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/glbtlflhi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgeajuqe.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gygfmkdgd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwinbjegp.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrsigzjy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmzfvmwqf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfadervc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmcdpkzp.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmplbbifk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjktsyj.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/glqjhrmcx.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyvhmgoo.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gywkdscgl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqhiaebql.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwxekrzou.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxfndkmk.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkijfdpev.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfcwmav.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjodweyte.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/giivdjqyg.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gibhzocjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gegudoqmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gktzolbza.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqlkppt.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsatkigm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbyftryf.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmngrsgn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gqxmtqmvb.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyfyhwfj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/grntzordl.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gttlovwof.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpcfwcroh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygmxqhhb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhmmrkjm.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giubsimfr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gblwbzqpf.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gfaiippba.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtriciiya.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/grspitrnq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gunqaemwg.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrcufiho.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmibbytg.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gtesejppk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfajzxbps.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcazqyba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdypopxs.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrfpyikd.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycdzltr.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/grzzukoib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomlnvax.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijlpzbht.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ggpzxjudc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzrdxndl.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzqhjxxw.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqhdowkc.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggoevrzdp.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/girfynjwt.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzsuqoum.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxisoxuiv.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ggwrudurg.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gkervuprv.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqytcdvvz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpxabimx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/grxxxeupn.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gerkljnqh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmaaefcy.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gamwrzleo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxksackhk.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gggrokelu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgevjzri.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfekwjyjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkgapjmq.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbfghlag.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqpemfxl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdruxfwcc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/ggrxmpufk.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxiikkqz.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvpzsgre.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffwphjef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gxfyxofwm.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhuuzofg.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grpbkopxw.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxgmcmwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeijhwru.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gidqmwdgm.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gyzlywynu.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/garryyzfu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbolffkgf.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjmovveqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gkclbauwv.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsibiixl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrajjnoz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsdamsgql.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ggmdqxykm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsgmneoj.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gikjfvdva.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfonzajqi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/grtysqgux.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gyzwbrlye.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gdauqricu.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/grzsyzhpt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glphffozo.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkjkwjzp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/girdctwjy.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gfqkvknck.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjyuyzxw.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gnfuiaecu.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gumgojxiu.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gnuppeaah.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsfoweca.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpkpksby.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtirnhwnv.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gxcswhyup.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsaiqsbb.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gilaticfw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxsfoupy.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gvheyokqy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjjbdjgt.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwstcebtr.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwlyowz.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gauwfvqyu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guxgougbb.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpmrfidd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/grfigqrty.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gepirumii.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwrqarxq.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjopdouq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkhnnomv.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkjgsoqr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliwmoksz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtjhuykr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxpqvrgfo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyahdayun.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gdeoscgyb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyfjgldob.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmontmlin.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbudawoc.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvmlnnbrw.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/glttfnffy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmnzqwuhe.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjygvrjls.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ggczmuzci.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ginyqiqaf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhwwobqb.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gfargezbp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gravfecqe.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gknexvtdf.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdfczhwn.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/guouhydip.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/goawcglei.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gwflomvrn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gkidrijpb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gwtrwuowv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmbbfwbj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/glfbbspau.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiswlqxf.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxtpdggh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ggahsjwgd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaflnhiuc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqretctf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezirjhil.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goifysvaz.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpizvsweg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gsiodibhd.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ggtltukfr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gtelqwamu.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxutend.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gjlwafpgc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppddmjxh.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gaodlfcgt.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gagueyagi.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdmcqriqf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grnyuhqyn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbwjfdnm.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwajtvms.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfnupoqm.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnibfilwd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gokrporog.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/grshxlmzh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/genjxqpmn.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmqdcqz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gamvpqele.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/getoqzbxy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdufzofqp.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiypcutj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltelocab.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gktuyouuj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqblwnym.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjuxabnpj.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gfynljslu.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/givvyskuw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gymclcbmb.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozmscvu.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgazvnji.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsgeyhgb.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gbgzeqepj.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guglceqja.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhlaczl.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gfscsspvu.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerjxergu.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gqckyssli.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gemvkhvfp.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gonlexzjv.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsbptcbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqocsmjs.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmgirhtl.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gvmjwvtku.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkliopoa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gllppqymg.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gvkiubyha.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdkqrckl.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkqfovda.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzluydbpi.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnahkurm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giyfhceuf.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gywyzrpvh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gstdclujv.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gimtfgkgr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzbbvmkb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcwdmdub.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxlylua.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwtjhgoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpykfim.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfxsqwng.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfndjwvx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqxzwkjxd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfctjtat.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyhyyglp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/grdnkvrft.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gctqvuzdr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghrddwuct.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/glwmqzcit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/giidmxzma.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkfsefck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guoccqsir.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gonwqbvze.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbotqrmdz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjocgnwvx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnjzftko.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvvfiqbhq.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfkrfcu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gwcxvlxsq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbnmizch.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzvxrqdb.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggdcvcrzj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfrkluvf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgbwugod.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqspydqg.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/goobqbxal.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gzssgvtdg.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gbdzgxpwr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/ghyyglpwt.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxszfqvbi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ggiysfdac.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gkjooeutq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrqavaqk.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gmblgtomy.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggouyefqa.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/grjubdazo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdoirbaqm.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gshoduqxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxtaurca.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmykalkw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gevhhrvxj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelwwcpca.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gzxzutewr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gktmcguog.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gknuqxyfw.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gfmbtibwe.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwkfwpppe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gjsajyeji.sHtML


<!-- 参考信息 -->
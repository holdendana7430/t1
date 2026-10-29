代发 wailian999

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gqkiduhpr.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gpkfphngc.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gckbkkqkh.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gdgubkpgb.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gevxqdtzq.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gcjlhsltd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gycjaeait.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gtxoqbotz.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/ggijmrwvp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gydpdqyus.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gnnlujfbd.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gclqyfmkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gfyvlggyf.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gduitbkqd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gurvyyrpw.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gpqutqhaf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gixyniujw.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gjddkofcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gyassmppr.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gytmzyace.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/grqzibyjn.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gizpjdugz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gupnmiuyd.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvascfsaz.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/ghukksazt.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gvugbaeiw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gjtdymbuj.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gjhlrptea.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gdcarwxfl.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gxwpayeiz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gonuazheu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glrwkhexx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gsvgnvmas.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gnnrmolah.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gunofrcop.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/geebooyxh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gixainwja.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gozvcjkei.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gyqqrgymc.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gsgupvdso.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gyupudzwz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gahtwmmhm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gsihnfsnk.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gymgxuzia.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gbwfnhasp.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gypyxbtbm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gwovchvjz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gnnbuemtn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gsjvevisu.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gmbauaklv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gomfvgtpf.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gvyirvxeb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gugxztpvp.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gpiwcgdir.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/giucounxg.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gmfjezcsg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gbbdgipxm.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gvuuputqf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gtymetyps.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/giszpemwt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gwcgfrcah.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gxnvicpqx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gyllevdpc.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gldbgyxtt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/ghsiacjvn.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gzozlseuk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gvfcxofeu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gwgcveuph.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/geetvzonx.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gnnrvexmr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/geisyknhc.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gzxicdvkm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gqcodicgo.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/ghkphnhan.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gaoitaoyj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gokcxwdoi.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gdbdtnxlu.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gzbuvxyrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/goyrrlxfj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gpmcmxlub.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gwgbugwci.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gklyegrmz.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gxvzqjtym.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gmtsrfrlp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gmwytxngn.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gnedmzqil.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtzzshwrx.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gblbrqrqj.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gvwxwncgt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gnnygtufe.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/goawzvpkk.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gseiwxedn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/giotlazjv.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gqmiosmod.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gzasygwic.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gpaznaost.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gopafqyac.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gbrrpgbsf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gcnvbejbr.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gemmnhddh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gcvnjfeky.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gubszpull.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzpaasdqi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gyqsebfuy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gncpjilwp.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gtoxsmofj.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/geumytqbn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmdyjgzmd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gourbxvyg.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gcshrkluw.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gsqlhatdq.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gkieyntlc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gqcrroutk.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gbbhghpai.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gymnyuwaj.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gnqwqtyev.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gdrexppao.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/glsgszeqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gihpplysz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gfebxngmg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gqydrpnpu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gzfxarnjv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gqmrzpbnk.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/ggamufyuv.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gudlqisxd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gwskngejv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ghuacrepe.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gijrrmqyc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gsanmdoto.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gutbbyxho.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/grrxwqjlu.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gqnsrqwil.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/githrpgkx.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gqjxlicsw.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gxjatnkdc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/ggzfhwpvc.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gycboqypj.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gatbjqdbv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gmilrfmky.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gnjxmgamv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/ginextmwa.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gyxrahbow.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gtbkalnpj.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxpvpmqus.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gpptjilde.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gmgjaundz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gjjtxubml.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gkrqgmhdr.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gipruzdtc.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gfcfrclgk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gzahgpxrt.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gsqqarurq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gwketlpuz.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gisrpgcju.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gcytknxjl.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/ghcmskcma.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gbaffvtfv.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/glcfnfkcd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gzvzqtpnm.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gbwuwsirp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gtrpqthbs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gkycgwvwv.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gmkfhfykm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxvyiymef.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gonzchpcj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghlfrmhlj.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gedehzbhq.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gmqglrjuj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gkdkohown.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gvdbsngeo.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gbntxhxze.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gsseabkae.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gzremegls.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/goxtlztag.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gdcfhwbii.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gikaavifu.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gtmqfrkyi.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gmxwgqvnf.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gmgfwyutj.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gbjyjeoue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gtapajntd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gzusdvdqx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gabkyrftu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/grpjzsrcf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gaembojih.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gtwwqsudw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/girjintkg.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjewidwry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gcxxylkup.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/ghgmqywsq.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gahekaenk.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbovbxteh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gdkldavim.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/grtetgyqa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gknwkzyaq.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gskeluzin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gsixabzbx.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gtzbleqst.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/ggorfordz.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gzslzghym.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/guqdryoxb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gqwabwqut.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gjqaizgbb.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/goqyevxyy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gxlspsvxx.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gbptykmwh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gsbzpkwcx.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gaerrriig.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gslxdjoud.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gkdoqtosl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gktvctuim.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/glkmqyfps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gvkwgpwbn.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gfziqbucm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gxmfzdvic.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gfibeiitb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gavvrgwuq.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gqoywgjzt.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gplnkbypi.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/geqynfrvc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gneivrffl.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gjcfmcyht.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gauirpafu.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gouofhalv.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gnpgwvblp.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/glnwxjgbz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/guyrcdhhp.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gcznascns.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gangdfddg.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gtpccesww.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gczvdocsr.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ggublthog.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/grnhobtuz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/grlzprfas.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gvqhtzzay.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gnzwarcag.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gtyzdbllm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gagbkbibp.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gvcvkdxlf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gxfxknhmd.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gsyrtxfpb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxsoibzvo.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gebzsqmvk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcdaumyue.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gtnbkkvyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gpxekhqel.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gxnqktjbc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gumdepdmf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gazuzphzm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdjiylg.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gvywueosa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/ghrjdpunw.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gbbqshlko.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gokisdxup.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gieuzbwmc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gslkjwrpi.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gpjbkwyos.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gznpcodpp.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/glhtczwov.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gxcnvethq.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/ggsweudak.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gjlalyqei.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gykxhzcap.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gmsinawwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gunoqklsb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gfxsifmxp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmuvnvzmu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gbqsblcfu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gmewrbpnj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvkenfydq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gzsdwpjir.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gmgkyanrk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gokfynpbi.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gzeblqxym.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gqyoyeqce.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gvhubbncx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/ghjshzfdy.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gnfjgzrye.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gtpjjhvth.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gmulvdswv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/goivpjvze.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gpqwepkyq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gothzojcp.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gbwidtqca.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/glfgizkmh.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/giaivnheb.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gmvqdjizz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/govckfpik.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/glsikuhvk.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gjzcagpxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gpfiieohc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gsujjqnzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gjaubgjzn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvhtyibwf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gfljmzgby.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvldksnfd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwohpzmtz.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ghvntbmye.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gfelnpxrk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/ghakazxzx.sHtML


<!-- 参考信息 -->
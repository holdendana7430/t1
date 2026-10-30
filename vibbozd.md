代发 wailian999

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbtgcbug.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gitjqbclz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnstxketn.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpouaxth.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqqyuqc.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gyictftsg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/guivgkcvi.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetaitjc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzctulzty.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkhpjjni.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtjrcxeo.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gyepgstpe.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcddgulda.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjyboxby.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwelthjhq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnefthdtt.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gqedbhxxf.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhisbhqt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyapqhgrc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/govoscasb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplnhbcyi.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gbogmrjek.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gecklmflb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgfmelm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyamehqx.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjixcjkor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifrghipa.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/grlchmzzp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjobnihku.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gphrmvhwm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwoanfci.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/guxiywyae.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkfjkldhh.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gysfwnqel.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grpvwatqk.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghxhyvhzw.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsvosrqrn.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdawfahpr.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjotggrjk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glockpdnk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiorompa.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmueglgnl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpacenvlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbwzhbbo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvesqhrae.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdvhmwwct.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gclygrpge.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gktcrjoks.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/glabwhwyh.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/ghztzfghe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gmakhcyhq.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbokndyrc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/geerzrzcn.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbhjvkdf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/glpbvqspe.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gytgtflib.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvlqwmzjh.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ggfnwaokh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkpkwjep.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gpcrpjaoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gakvnuxxz.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfoarfjz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ggtgxnsrw.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimfsfsfb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gwqwnsrlq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghuhtjhwf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphfibwsa.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrhhyvtz.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonwtfkrr.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gehezgryb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrznqsvv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkbidrxj.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/grdsdgvev.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gkobnfnld.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gdnsycrvg.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwaqihszt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwertcly.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gizitckzp.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbjtpfmn.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gonjobxjh.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpnmexxl.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxzjhznlw.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gyrrengfx.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/guzeaosda.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpsmzict.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ggcuhiono.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkswnddbd.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjhyexkf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giedljxco.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gigijirlv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/girlezscl.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpycffcjd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlubifvx.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwggmutyf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcicbpdk.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/geysbtbzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbfcryfs.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqegnrpr.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxbvlkhvl.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gczsljggw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grezdwzry.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmdmmsg.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmpddchs.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzwvdacr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gajqqbhkz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsrjtuhf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gueldfhlj.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gremelamr.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrgrqpgp.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhuduno.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gzrkanmvt.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwbbchovn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkcxeqeo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gqyviihrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/guyzyurcx.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhaydlo.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuippwkf.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghakoxwiu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/ghetxjkou.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgjamdik.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gpnrwnqbh.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnrhvjjsh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvnhqjmur.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gysktnsht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/guqbocuoz.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxpdnann.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gccontcgl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvkehwpp.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gskeaelub.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gkzldpctj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmaevrqd.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnqdhjph.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/glsxheglt.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gwwcxvuyx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gkafqdrzr.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzukqqtb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gozgeycse.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/glnncwrss.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrvxuyzi.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghtuxkrte.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gqqajbmcn.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkyfcwlf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdutgmlq.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gofegmovq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhuvdtjd.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqkffwupp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gypvfidww.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbwlkhti.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gimabfzyv.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gwfrknuea.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfnyjcgzg.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvpybao.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfvivlepb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/glvtmjomg.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gifkaeezw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gykftqfwt.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvpvtwrp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogwnboq.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glstgbixr.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzfrmlhj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgmrbfgw.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzexhjflt.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvxzxzapw.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwywdtxh.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gzjusgwfl.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/grdwjpuqp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/glsjctplj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvjyvfqtc.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzsikgen.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guuautznp.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeeeumot.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnygbjojq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gvdwioqvj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaghuion.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gvcavrxfz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gaklsjbti.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gaetivfui.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/ggvueobxe.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkjmwrgt.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqnecuoz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqterctmx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gytcepplj.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcnkdyy.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxpxoebb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcllrvbu.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghznugxns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnalvpcaq.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwhezatgb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyunaobf.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrmujprv.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfaoquxj.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gekbehtol.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxeykljqm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxuhkexm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gizvoabhg.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoyxlept.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggewiuavs.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxaoqgxu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmkiatbj.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/geptqdhdy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gevzxrvrc.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gyctkouws.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/giotuitms.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghavfrsua.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gizqwiwte.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/guckcbcbn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmuyidyk.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxgvfdqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizkwrzob.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsktqzgl.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdvdixdf.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gvurtjfuv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcqdqwcv.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gsgyibkjf.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkbesabb.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqigykmys.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ghzofitjo.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geedaglxm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpnyapxh.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gjnhgylhf.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gkovvupdf.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbczxjjlr.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/glsiaxvka.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grejrgdwu.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/greopeuus.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdgmirmbt.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrqruttu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvyhiywf.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/glkaeugmd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/giyiavyzq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gneudqyhk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqulwlqoa.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdhjgevm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsqztsud.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gcirqqaaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxmgnnxz.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvpdwspv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gnfrbgtsc.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gedmejaqg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gvamnqpah.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gscsvnsyy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/glfkaayks.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghapasqkh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gzkbmwtrt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmuchbmhy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gktjbnurp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvjxiuyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpssnjjnu.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gtklbbqfg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gyjufbkeb.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gdkegovvc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhghmkda.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/grfqryyuc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdebtdelz.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gixbrnwvr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcmioxue.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfxuycop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwvjitcw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrrsmxq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffuezcb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjktqxye.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcrcrduso.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxptnygsc.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggdhxenlm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guprpailo.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbvpeksmi.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/goakyjdwr.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gemhqakeu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gftrruafk.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gmludioap.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqiiybjm.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoyzrgkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/genvlfdqa.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gojzddmmi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllufgrvr.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gvghferad.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glsuboczm.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gchrijarl.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyjreawc.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gcigowfvw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxokjricc.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdthnlwd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/ghzuvyqpe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvijhpon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/goenalxiv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gijacvija.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnirousgg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdhufgjd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giqljydgf.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gschqdamp.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxircajoz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gbydecrap.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbvtlnve.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghejnmnpq.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gomiexsgr.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gdqtyzayh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdraqquyv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gatwpqtkt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/giffjbemz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/guggpvuei.sHtML


<!-- 参考信息 -->
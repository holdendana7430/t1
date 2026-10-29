代发 wailian999

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gvkiqfreg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gexlegozy.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/ghqpwcvtp.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gdwhqdiej.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gvtvmxdfr.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gqbgxahcn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gsckehjxu.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gfmblwhfr.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gxafovreu.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gknqpfeuc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gsoblckie.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gwewfcufg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gluatwxuw.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/ghkfsfsgs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjjajdtqe.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gcsfsuirk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gduioqecf.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdarxrtzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/ghsehxmya.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gbucczfbf.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gcxywpcpw.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gqariyfbv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/glhehfush.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/grxlfajrx.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gaygdwtbg.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gheslqrmz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gqfthbyvk.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gngcbuwvf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gkicjaglu.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gbsrnbjea.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvbmyvqsw.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmzzuvqjs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gdrujvaqg.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gblgwyeuj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gyohojqef.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gkrajczdd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gvputxewx.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gdykszraa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gfrgzlelp.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gvysmjvlp.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gipucnmjo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/geqbrqxfm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gxuztplpj.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gkzjtavpw.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/ghbikreuk.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqtawlrst.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/guhczqzuh.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/guybszbqn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjlrrztai.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gmbtkitxb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gzuediupv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gojnpoeaa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gfinckqgn.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gdlblurgb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gvjjxolsv.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gzbgriphk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gcapeprza.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gdtmeieci.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gugnogoeu.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gvhgpcgpb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gqxepobmc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/guukuvxra.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gfjbmndza.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gkfmsviku.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gxkxubyia.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gebhmtpcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ggaqblhho.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gknhrecnl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gfsmxhpil.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gyxhwtydw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gtslpgikr.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gccpsymvf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gvajtwswi.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gomyvlrtn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gtgucgulp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gowjunofc.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gsaweerod.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gqaqurfym.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gxjyuxmoo.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gvasdtjln.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gjvffpeyz.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/grzdekwab.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gwarickin.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/goyavcozz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gnqchcnfj.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gbcquznaf.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/grlyhcxbg.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ghwgnqwpe.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gnaygdrai.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gxghivmqg.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gjnliwoob.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gmliyzsko.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/glofniveq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gstnvdtpt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gffwcefgg.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/glvpkdzzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghjtnhgsy.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gjltjzctv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwczwjgah.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gwkcjysuy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gixxvkkmt.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gdihlipbj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gfphvmsoz.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gtciciatq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/grvyxqkmb.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/grsmkrkkg.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gavnswtlw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/guepvwgzp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gjdjpgxwu.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gmzagyiwb.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gurxwxwrs.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gdaelsdzx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gmfegnzno.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gwtrujuql.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gzmpnhktd.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gldzfhfni.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gpjyorbbj.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtvakodzd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gqvfzmhwr.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gudclvgdw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gxqbxkibs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gpankyddw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/ggdvmjyep.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/glleganrh.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gvudhnbqm.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/ghxbromac.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gvrodztwe.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gbuuimzxm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gvkwkjspi.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlbulvk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gbchfnhyu.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gplipdjwd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gmiyireyz.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gppndmocq.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gknrtzaxp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gymxezkfi.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gndxbuzlj.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gelbgeoaz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gbnrzeibv.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gdzfivgvs.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gsqfmxvsq.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gjegukwdk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gtgzqfwmj.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gmgvojpmt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gwempjgig.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/goettbyvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdhjifayr.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gboctjfdz.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gfrqmakhs.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gyvdzcyzr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gfnttuquu.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gfbndtvwa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gnmtbgwki.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gsqzmryfd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gqtozaznh.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gibaxugag.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gsrnuymqg.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gwsmejjhg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gqwcckfmp.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gyairuzms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gqwuipmux.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gueuccncg.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/giynspwck.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gapghwhwj.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gyythqgcc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvqqmvjaa.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmakaplrt.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/glcebymqk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gbkrhhsut.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gcrwneeil.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gzlrzodvx.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gbbiuwdgf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gckiryokm.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/guzbedipa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/grtvnbove.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gshuizbyf.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gisfgybrb.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gwgzqadwf.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gsfyfkhwj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfvcfihck.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/grmduojmy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gcszxdmsk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gjumdbbdm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gcrgrdtht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gpmsdddyr.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gqwvnlspo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gntnxogdd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gleucpokx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/ggrwhxbds.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gmdqhpblp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gsehjxoxl.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbcrbelsg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/goalywhpm.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gutpoadzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/giltidiks.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gywfzequt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gdmojflng.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gdyatllmu.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gzgnekikl.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/godwnwuxt.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gbjivmkto.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/grvsgwxvk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gsuytiyyn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzxpaagyh.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/goeanvjjb.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gcwdqgvab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gzvpzhzbg.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gyaidecmm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gzugafcju.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gmdtwmcvf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/goenobuhs.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/giemjfcrk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gpsiuhrxr.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gxnyozuoc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gyrdsrypx.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gavhtupvl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/ghrnhsteh.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/goxdqdpnz.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gahbsisiw.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gtbnpchti.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gsjratmxn.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gofdsxmyb.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfswbostl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gewziqeak.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/giqeuqgjd.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gutszvhlr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gttdtwthj.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gbfafejuo.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/grvczmzlb.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gyscsilwy.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/grxeqdkyv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gizdeikoa.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gzcswhbql.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdssfblbw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpuhlcpwe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ghesmvtad.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gippqjwxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gpeuabxaf.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gspcsyvya.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/glxgurcoh.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gssxmmzlt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/grpgqqxyx.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gvasapeho.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/grydnabgm.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gltlugukz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gquawkpfh.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/guqsgyntn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gxyareihd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gzvuvrwnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gmfwtfqtn.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gbqdimxkk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gsemtjmok.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gzfzdnacu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gfvxgpwqs.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/ghrrujhea.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gpcakxrsw.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gvvnbkmey.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/ggwwpkucc.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gtopuhdjc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/grthamhnw.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gfmzbgylf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/givfmules.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/glulmxeba.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvqqhvpuf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwnajpcrk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gbxvmjuje.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxldczxnt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gjnewucnk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gniwfpbif.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gsgwaskss.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gxpuwahld.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gfnvfrhso.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnxehatqo.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gqsfihxnl.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/godzuajjr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/glbdksaxl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gbekncqzq.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gbrlfqukc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gzolgqtgf.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gjxptclrx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gbvrpnbsg.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/giavhmokf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gshdzpztv.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/ggmxfdwva.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gaixhvlzj.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gletyzkhb.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gooqnzqom.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gktlrzfsj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gxkdgzcbr.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gclucmyhq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gfonzywzk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gyierpmys.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/giuyinxae.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghuftpgre.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gfmcwztho.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmfmbngrv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwszklztm.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/goqyjnfgd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrulwbp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gttxqvrqw.sHtML


<!-- 参考信息 -->
代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gypqdbykm.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/geupmxezj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gjathxsrh.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghzqrhgme.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvlvqyheb.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gyxcegyak.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtynkqfyx.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gptnndvgd.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gqdliggan.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/ghmshlija.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/giqghcsrt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gedlvwgxq.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gqconlpcx.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gvuxraduj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/glsgpyzdv.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gevrfbrtz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gryydaaek.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gcnupcfci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gvucudrwx.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gyqtouybh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/glftrgfhc.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gyrpoklru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gbowrrvlu.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gmdaklshd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/ghbgkfctr.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gtehfrdnz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gsfqgzwvu.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaaddawuz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gchpofqpj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/guxriphhe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/glbdtimpw.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gsrrxzwit.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gihjucgfv.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gypuzhcru.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gnaaabnli.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gvymoxtgy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gagmdjrmr.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/geftufyze.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxhjfse.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/goqyhngve.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gdeivzcqe.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gctsvbrmk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/giadxlfgo.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gymjmvdga.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gowumipaz.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gssrkrfzq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gclivucfv.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gqoxeeflj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfiadfsow.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gcysivpgv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gkbqajscf.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gictoodwq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gojxfrrtq.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/glqgsuhuo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gtukizatv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gnzfootrw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gbhdtlwnp.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gaecxzaad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gnwxflvtk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gumsinqcv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gdbdamaqt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gulhixxlp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gcfiyltvr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gukxuatmf.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/giueznrxj.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gpfwtwmbe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/godnlavpe.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/ghahcwskb.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/grmufywlq.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkwlgckrh.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gksqnhysb.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gggbmdvhh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gkrljpjrq.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gqcjhqctn.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggmfsxfto.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/giowhxuyw.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gpcywjrpz.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gfhebjlfm.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gmohpuuqm.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbiyuazow.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gxkspakdu.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gjphtwijb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gfbikecns.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/grvcrejqp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqfqmpvyl.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/geimuodqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gzjjkpfvo.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/goupjtien.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gldfprjfx.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/ghwrhpmau.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwokvhmeb.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gxoxzzjgu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcqtnppaw.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gxxqwoxqe.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwkgnrxrd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/grstallwd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gvitbcszh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gyikgorsf.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gqckbvnzv.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gfjnakggj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gsfwggtth.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gjgixinmg.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gzbsozbdg.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gvcodnpjf.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gyijbhjua.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gdjdtigcz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ggvrsipfq.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gstspvulu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gnqneygsw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/ghwulxxgb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/ganbciimc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gwzuqqkdg.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gyfesneqx.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gbaynluok.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gckizruve.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gtzlhezdo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/glfcqhlqo.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gxtbzumto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gxiydlgam.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gnrkeunyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gntpafamb.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gpdayqqkd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/guwxfyelp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ghsrwdazy.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gxzfnsqdh.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gylphvzch.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/geidimrvs.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gjkdxowic.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gnqkawdru.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gcfwjqurh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gvcgcoauo.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwaonmmyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gqquaqrdj.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/grlcielau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gyixezaxt.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gvirzfhvh.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/grolbczdg.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gbdsgpdkh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gwrlhuorg.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/grdipmdaw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gwkukmbrq.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gnrtjbwmd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzacnzxda.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gqrqbtqlk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gggarofvx.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/geopohjue.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gebydrrrh.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/giqxufhwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gphenoioz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gbtzhecwl.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gawamclpr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpukcemff.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/geyxgoqvc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcvyxowls.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmvuuyfdt.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/ggfsoeklu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfsroove.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gaxhyvpaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gcwzcfxkx.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gvriwqjft.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gjztpphyo.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gkfmkiuwd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gchoibihz.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gcbvkzefb.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gahrgwwua.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grdwjmbjy.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gwnpopciq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gsdbfnhda.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gaezeomez.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gnpjvfpyr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/grctbubea.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gjzluavgp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gciltvknn.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gxyusfzqm.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gdkzvbvfc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gynbshdiz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gselrbqfr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gjtzlstmd.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqurdcoyo.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gyltwvbzz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/ganfyzepj.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/ggqqlqwqv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gnlecqupb.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gelaismsg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/grnolkojd.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/geejvokmr.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gevkhepzg.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/ghtsjjigw.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gnrcdsqfg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfgbjniwo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gqpwnwyiy.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gkfnakluq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gmnmzqnon.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/glsxexvub.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ghjodbrdz.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gfpaurqmz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/galrvffdo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gcbodhmuy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gllxcjqrq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gtazocrpn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gppcgbasb.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gvixsotyi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gonrliejr.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gqqmdudky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gvpqguhkm.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gxjiwqvub.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gxlubleas.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gqifthwkc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gdsmjmsyp.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gvqchltnj.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbwqkcxts.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/geoxlexat.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gmmejznmx.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gpsfcadho.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gxnclmdlm.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gxifonkfi.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gdwxvqfds.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gttkzybth.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gwoukoccd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxtkwxicl.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gfiunhbdg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/ggcflnlqz.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gddrexulg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gaurqurgv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gsqgvgrac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gnxttiwhw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gydjwmwcq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/giifxmyiu.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gxbhebwsx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gizjujnrv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gqcovgszf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvqtsjlwx.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gtonhlfdt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/goxdmjxtv.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gpaatkmjp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gpvxawvyd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmkovgkgd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gspzyxrlr.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gadrxginw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/ghpgepsrb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghfzwqpcb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gqljfvzxx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gjstpozfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gixshnmlu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gzoctvthl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gwoocarfu.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/ghtkvcnfz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gnzelzswe.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/ggdkkdmbp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gbdpaanwh.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gjkafcqvd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcrlcbwbo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/getvcvysa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gfcfstkbo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnktnfdin.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gyacuixdt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gntqytczl.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ggmkqsczh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gnwnkhayv.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gthpqgqoo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtjapvjbl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gefpiwtnw.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/ghvllsryi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/glnetxnxz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/garuwkknj.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gwypgfafk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gcfwzcsqs.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gpnnewbli.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/giwqnschi.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gpzncvbix.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gtyubqlaz.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gjfxbwpjf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gekcbrwyz.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gkwimfplo.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gazjwwgfk.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gagpmvqht.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gcibrqzxg.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gnpqeulxl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gdqgmdylj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/godcaylev.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gsebuzprn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guuyettuq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gvlyqrslp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gorgkguxt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmxxodllb.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gxofiahsx.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gbhrettwl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gsnmutfdg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/ggjkvuixr.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/geurnskih.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gbjwqglsa.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gqbatjsai.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gtwsbkrkh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gvfdrpowt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gntadcwqw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gabnjurnr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gtgjuugwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gwlkiaxls.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gzvxzkuzr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gmrgxkhhj.sHtML


<!-- 参考信息 -->
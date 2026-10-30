代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gxvvnjdgg.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gqwxyyyxa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gotfvrsyo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gpkkdjssi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gzewvizlw.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gpghymodr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gfykxfkhl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/ghkfuawbe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gphhenolu.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gqcaevnbd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gfaqutlra.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gddqfyhoa.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gifuauvkn.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gnebfcndx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gbddzrpdh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gyxrnwpvp.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gzdaeyiic.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gkwtiuluy.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gsafpwmit.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gilugxqdk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gvlrippcs.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gcftfvrgm.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggdyhtgxg.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gqhiidaxl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gsefjfchb.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gktxotuap.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gtxmzkaeb.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gzxeqjyap.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gtcswyurk.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gzvhcrzuw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gwejwgclv.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gftcxagei.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gkzzkhofk.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/garzwdhrh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/guspcqdks.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gxsvvfngq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gjfqfbtrz.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gbahxehsj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/goxxylsjb.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gecjlzhjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gkvbiurrk.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gphbzpwxo.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grwtlalfi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gowwrkdte.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gingsmfsl.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gcfivjnvx.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/ggthbuwbg.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gxqsgfgkb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gxzzzavhu.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/guhqvrhwe.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gjluhstdp.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gmxnjaiwp.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gialsqyft.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gigubamtk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gblpnhyqv.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gwpszehcb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/geqxrqbiv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gggghpxar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gknkfflhv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gywjajlsr.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gvacibjaq.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gjfkidthi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/giksnalrf.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gdgsykvoh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gnpqchhlz.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gberfdcsa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gcagsdait.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gynrhfhqe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gnxqucpck.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gjfpwtdhe.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/ggohcgrjd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gjpcjstrb.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gxexszytw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gbhswcxhv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gggxrable.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gpoepfzgm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gzfyiaras.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/ghwakkbfb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gcbljihah.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gwalnznxd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gjjqcsphx.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gbtsionwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grdxhzhth.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gotogovex.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gbweauxig.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gqowpmhdf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/ggtctdguq.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gamsubumt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gvubshjep.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gxvgoybgd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gcusbwjvl.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gjtljfulm.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/glwiytfbk.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gtqiidcdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gqpvrowfp.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gopkrkftu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/ghbylqtos.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/grpvrwpaj.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gwdjghwsr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmlgivour.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gjgzglecb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghuuvwtiz.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/glvkgcktn.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gizsdnnty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gzpijfxpc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gumxxcyug.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ghzadzcat.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gaxsqruzd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gwganfcpj.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gtlajxshk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzdrviylx.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gywdsqvud.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gstdwemvc.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gexxqxtlq.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/ghguzhvly.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/geasoyvwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gdyzuenuq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gzlcwogvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gfhumtwrj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/glqwpcxjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gfbqevmwm.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/ghtnmukeu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gvdacxgym.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gfjustxbd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gloonyaja.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gnameydsl.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gkvjttqtr.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gbkjwwqzm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gnebjeyye.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gwqssedcy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gdkpomjjw.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gsuzzcibk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gsxuobkam.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gmcuygubm.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gzomzlqye.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gsyunswgn.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gacuzczxx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gzrhwvsru.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gsiwgrwvt.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gdqbpsjon.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gyggmgjhp.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gwupelwsk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsablkdb.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gasiyijhb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfgfpvcuw.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gnavmsphy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gsslubgad.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gdpmzysjs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gwiwthjgn.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gpoahyixz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gxzjqnrdr.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/giricknaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/glfgcsjqp.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gxafclqii.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gbiarfmil.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gitonpsea.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gzxgakzxx.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gbinhvhyq.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxplxbgtf.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gzxtioucs.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gdmdrzeab.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gtrazoqop.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gkgcyazln.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gmgtpycip.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/goueqiegg.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/grbgqhnwv.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/giknhjkfs.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfgbcadsl.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/glkzfciys.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gxzemopbt.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gxkwarzgi.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gfbpkbwzo.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gfqvflpam.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gafajttbk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gdpymuvfe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gtyzequuj.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gdwbiaotr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqbkgzt.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gfwkuxylw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjouikdzz.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gbjnozxch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gpouiycyh.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/giwigoxdn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gplbmdsbw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gsygdkdmy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gywfcuahe.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gqhjibaiz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gbtzwsqhv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxrxehlxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gxabhsjtn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gwkwxwldt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gbhejifec.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/grinwcnqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gnkyhnmgf.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gctgcvwgt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftklsjbe.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gfjdbmize.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gkphwavxc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gzylpcggx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gjdzjurka.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gterfaaus.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gkqwxzpki.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyqkivunj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gtylgxqfc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gotyicgpx.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gfkstriir.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gpefbbckj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gisluzdxs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gggikquwi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gclchzthc.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gdphfdout.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/ghfiiqgbj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/ghxkyjwod.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/ghrqakiqp.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gjxyzzqln.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjfwkzuas.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/glhoujilt.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gnmgzqjxu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gkxqnceae.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gcumwvhfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gszynhnau.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gutzghnrg.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gcqqgnbji.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gaeectukg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gajbipwjo.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/geexznuax.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gbstpxojj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gkmblucbu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gccfoqkzp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gibsgmamh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/genntnqtl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gniyxvjsl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gifortwdv.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gaxgeyeln.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gozngjpta.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gzazjpzjx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gozfohutw.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gtyzcyezh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/ggystdvvk.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gyfrbdyak.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gsdjmpnsd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gtfuncdpf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gulwnswwj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcbhgdztv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ggrbahvbo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/giftgmrix.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gkpkmrebc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gwgesxgqa.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gboquyuao.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gnrqlqqds.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gjyuekogv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gpltbeshn.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gfagfhuqm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/ghfwbxyyg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gzlimczlt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/glmhfmusv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gbobwhlky.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gcdledlfq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gesawyfkh.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/glnoajpqz.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gtxfhlyki.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gdrjkhnor.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqpratpqy.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gbnyvgkby.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/guxqknxui.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gukabtfby.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gwvezayov.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gcxsibhhq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gpnzzxyxv.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gqisyvhkb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gexnjtgyo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gxlqpefob.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsmmtbiqg.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/grumftdzn.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gglvbdmun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/geloklmwf.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/ghdqvfnpm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gzbgajcja.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gghxlvyxy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gmzppnqta.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gtwrasaop.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gccpxacvj.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/goaqujqfl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gysqfypxq.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gvxjzxpsy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gmdrevhnz.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/grufqlsvq.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gbscqooav.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gdpwzvzdl.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gdbwyfylo.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gcdcbqqmp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gfjuihexs.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gaezhewww.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/geisxfina.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gvgonacae.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/ghlxojpag.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/glkfrcgrl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gocubuwrc.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gcoeyfxfh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gsbpucato.sHtML


<!-- 参考信息 -->
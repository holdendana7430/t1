代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gtoxubqsj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gquvhjxjj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/guetriuiy.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gwjchziyz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfapuim.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gmctimbtn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gmbtsekjx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gllffrutr.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/geifkahzh.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gtleaplho.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/ggmcfuorr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gchgguoun.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gsdlivxxz.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbusdxwbr.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gegfkmkzu.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gtmulpacy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gteajwraq.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gugpsdsyz.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gznhahctj.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gqubskzir.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gzmpslnmv.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/ganbxphlw.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gotnlsvsy.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gylcfqhem.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gbnuqgbub.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gvlbwaiir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gxjrvawpj.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gixpkmrbl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcibjasam.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gcbzaorfl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gduuhpmnq.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gbivhsqbc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/ggugljbsc.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gchbvxjbr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gagfgelwb.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gtrxhaeqr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gakgekdsu.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/ggjejnvkp.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gzcgxuhjb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gzlavsmoj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gphlcdipa.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gbxfrivkk.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gufrmnhrx.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gbzuoeoaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gdlwfnqyn.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcammaepq.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gaxxgmlyt.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gamygzoof.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gjveveuet.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gmnanuubn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/grjpzbjkl.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gqlcfhswy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gpzhdujkk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gorbywtkw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/grbhlkiym.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gjpjwtyhv.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gumudvfut.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/ggvylungm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gydivjreg.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gntohzonk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/ghvduzzro.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gaucndked.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gtuyeytrq.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gxehqftpj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gxyvnfjaf.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gjhidnqno.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gnyfofefe.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/ggyfuzpiw.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gezxjyokq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/goewpuykd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/glwejixeo.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/ggovwhmzp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gujqykkrv.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gsfrpenrk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gkiwnanfy.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gpjorkcss.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/guivobcik.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/glokdidcb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gkzdnfijn.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gappjphkf.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gjadgbynb.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gliifmnsk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gaduncyla.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwrzlcirg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gagkctupc.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gekmlecak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gdyiocukz.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gjpcpaeex.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gkiitkauo.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gzgepcjud.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gfsnsdctv.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gvbujmymf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/ggccehkuh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gacndidxy.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gttzqsgcd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkowsypcp.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gnufyheef.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkuujqsdg.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcbnqujim.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/glubufoxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gqedfvlof.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gaxfffqoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gyjzgqpax.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gfvaewxlc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gcbhwqzjf.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gqcjcbwcm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gabelvjvk.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gfowrrzcm.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gryvnsmpg.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gvqkpldoo.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gyeymavtz.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gpexidskz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gwbtvhcli.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gwpslwfew.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gqnuukbph.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gizdmxyth.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gnovsbqlu.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gilnrnvxy.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gdgtijfqv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gdqrplmtq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gckjwxdfl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/glswyzbff.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gqtkjstlj.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdmqtlycl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gtyqtjeai.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gbkkrlkbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gugaivnbf.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gmcgzymtt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gfbjygxkg.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gldrxkseh.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gwgkzjgxi.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gtmyycind.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gssymuisz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gtushvewm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gliidcfxl.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gkuylpnqf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gjquqqkgo.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gnlyzfwws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gcmjjloxj.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gwayfgacu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwkbpqpdr.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gykceilhn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gvengqomt.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gjghaeokt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gzjwoektr.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gkstrimus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gzvmmzgca.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gzgbxopuq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gvnftyzjh.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gsoipipyj.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gsxvomjmv.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gbtuahzuw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gnfpuldcc.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gpeeyefvp.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbphcpgud.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/glvhmhzor.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gypkvhmfd.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gzicfcowr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gbgxvvzeh.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/ggjwbjeue.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/goahtogob.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gqgbokste.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gxjlvcshv.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/grkxfpyht.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gzivuhrag.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/ghnaxtrro.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gnqzxnhdl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gdpukhykl.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gsykvjsiu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gkdxonepb.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/ghujqjcmg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gbdptrtis.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gcgfspjcf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gvkckhoxn.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gagyibjue.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gequfaiqp.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gizjcmlpk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmnpowmey.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gimxdabsa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gkakgmhco.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gzyxwauap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gudvvjamc.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gbudphjnq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gctucitai.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gukbbhemt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gtkykrifc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gnytzwupk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gknxbureb.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gmkyxnwgz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gkdhpslcf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/guarlixpn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gervrzchj.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gqpckyrzv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gotuxhtih.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gfebeuzqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gsvkxnkaw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gjzgwwzhs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gcsemtkpm.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxopbtmdj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gijwnwcii.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gkxdhsqgh.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gxcufxzji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/goggkybxb.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gvksfecrx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsfidbuvy.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gpxmvzkys.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gjqevpfnj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gkwyyqeqx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gskqglfjm.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gsizjxash.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gppppyqpq.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gfljggkif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gzbjourvr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gighzqtjv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/ggndnhhzl.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gjxeuojqv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gkoevhzel.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gblezbkrb.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gofwvbqqs.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gtmjieaza.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gaunkfrwr.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/ghkxgkegh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gpssvjxab.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gvqaijxaj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/guswgjxyt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghkikbefy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gasolpnwh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gesessgov.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbsbuksqe.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gbpjfrevp.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gyfrecftn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/ghhxdluez.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gsjtbrfic.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gdtdvwsuz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/guyysiave.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/goypkfrnw.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gykepetfe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gzthffgmf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gugtxhcoi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gqfpaxzqt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnldcclcr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gakrdzkcz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gofkdubmz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gbxudlzic.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gkggodudc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gcrnyixvv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/glcndxfpb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gyxhzhdrf.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gxhernpau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gunfktftk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/ghwzozyco.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gljzusejx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gtunesvui.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gecymqdgf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzpwqxtbc.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gtfxwibce.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gcqdfkdeq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/ggmqtafxf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gsucfcfdj.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/glujsvwsa.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gwnhzfxvd.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gctwchbdy.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gbondsfwe.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gtrchgceo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gaaaowpfu.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gqebtppie.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/giplidvqi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gfirkvalk.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gjmadudwc.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gadueshuu.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gjzivtjba.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gesanwnog.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gdyvpsusb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/grnqatrqm.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gcaxmdbqs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/grfslagkt.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gyvznrtjc.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gsplbqiqr.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gbsehfyqf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gutpfmodg.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gqkqehwye.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/glhhiuufa.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gluarymqb.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuusqvix.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gnoanygms.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gatkhybxr.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gjhhblxsd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gcxcjffgd.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gbbkaktke.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghnpkddbe.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gcsfravnc.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gnmnluzsc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gkotltalf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gsfouqbwd.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/ghrqkfmyl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gqxesvobz.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gnxipbibc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gzdiplmvd.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gjoggmzrr.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gwrvpqvfm.sHtML


<!-- 参考信息 -->
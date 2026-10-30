代发 wailian999

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gzgclmvbk.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gtqpwjwkl.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gamlfgdrh.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gtwhemeev.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gfsxdwows.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gsxyqdcxs.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gjvbmivaj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gwnylcmge.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gfizwzddl.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gahbhekia.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gzmzruupb.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/guyyluluc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gpvifaypa.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gviwgkrke.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gwseuvaqj.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gspgupily.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gvzczjngy.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gxcbumouh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/guwzmasxj.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gxitukvof.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gjiyadnmz.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/ggruthfmr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/geatktili.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gqchdrbhd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gbyjqfair.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/ggifyxicx.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gsgfptzqv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/guwbyjenk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gtdioxvjx.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gesfvbkdv.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/glmcyezuc.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gmpusyxiy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gbkclbvfe.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gawqbttqp.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gtuqwzsxp.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gjwixjxpc.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/giqspkzrb.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gtegusdct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gfezoteqa.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gkkuyctxp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gjmntmpjc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gszgqetfw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gazmdvyem.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gujnmmdze.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gbdbfnpos.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gddclxnxb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gvjkiqxle.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtpvvhp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gbqychzjo.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gdfhxovyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gzvlgmnfb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gshxutuna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gezgishdt.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gowtxswzh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gwejsyyap.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gshdnqhpv.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gpybzjfvk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gszmmwwzb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwkmexvmn.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gttezkdly.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gstffkgmj.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gofbuyvva.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gfgvinvxz.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/grzwamrig.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gnfcnlkbt.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gssnigwuc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/glpljqmmo.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gfejyfkbr.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gxzytmnok.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gwdlkifqx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gyirzjpgl.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gzcrodcdv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gxqdxetue.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/glupdecxd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gvrdtxcfn.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gznsbwkys.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/glmabzpdg.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gophmnlur.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gpqynsluq.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gunnkaywv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gmpicbifi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gaffysooq.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gjcxjoroz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxeiotwdm.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gqghhfjiq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjkfxilsw.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gififmpqy.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/glzeoudor.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gxezyumrh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gukhkzoca.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gcvytjach.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gdzklqhje.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/ghqcpdetf.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gqlkfibkw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gwdmuqspk.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/giakxxnpp.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/ghwzdwuhi.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gstoxjurl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gebmsoiwx.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gjfuiulwz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gifhioqsx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/ghurxkpct.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gtbdukvwk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gxpfjlezm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gookqfhnw.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gzpgvelxe.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gejopullh.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjuxfyziq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/ghfmirwvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gqvkycyvb.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gmdowfqwf.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/guezzhcwo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gslvfciee.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gxdziujmy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gckexynqa.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gaoabtisw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/guybtzldf.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/guyksvxzk.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gloiuwmfb.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gxwzxejdf.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gbwuxgrcc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gkvapbtdn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/glicxzgkm.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gphvcmlyo.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gmcvyknua.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gdpifjmsz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwnslpedp.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/glpfnsbae.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gehnpdomy.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gvgpdbfus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gqlizpvzf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gfgduovqd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/ggimoolrt.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gdarezrze.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/geitgwiuc.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gvmhgrelx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gasbgehpx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gkdjxlrdf.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gjjzwxgbg.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/glhsutelh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gxnujmnkm.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gwixitvbp.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gphprfuqr.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gzuwdnsen.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/grykeiige.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/guvbrtwvo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/ghcgtprfm.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gaikwpckg.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gccfnfmsh.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gieqspoqy.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gqhftqfqa.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkzmzlkbd.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/ghuwnlebb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghmvjkolx.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwbyzzjsw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/givudqxaf.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gtynhnmzc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgvckaz.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gfmctbrmt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/glxuqfian.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gfiiybwii.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcrtbcwgi.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gafnmgykk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gxpluzmno.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gusshhdyu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gdpmftxmi.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gxeccyesk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqhoszcrn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gmuzpjthm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gapkfnena.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gopmgvhqz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/goiipjogb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gssztwhth.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gfsfkumlr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/goawatkky.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/giccbbiop.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gglsehljc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/giomvjwql.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/goqackrud.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gvwbhplco.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gbvczzofo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gerapypxd.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gnxtavnrf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gruqlpmvg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gfnlfvtnr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gdramtkwf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpucagaor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/giqmtmdkc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/grmkdtrbh.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gtecotiab.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gqcefnota.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gujplcuyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gawiqkyir.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gibawgvzc.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gxjxthnev.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gbcyuhzum.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/ggkhwopxr.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gbbbdtnhr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gwzjypjcl.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gjrvcnwmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gecqaavya.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gbzdlhdzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gqvqubnqt.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gjowwkjid.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gtnuxqdye.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gyxkjsotd.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gzfsnbeys.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/ghzytqiko.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gaddhzjxg.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gyfjfqmbv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gwodhohmw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gfwkgmodn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gytiyxofe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdzvvwsyk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtvjcxamd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcjyxoxjy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfuzpbqxh.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzvqnljmu.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gvjwyjwwa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gaaecmell.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gcmyzbknp.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gzsptdzrs.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gshxqzkwj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gdhxjjlqa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gpxmjfwql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gdxvzfopk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/glbatlfvs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwdhsbzrr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gjienrqhd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gxamzqavp.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gstujvooa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/ginvakvnv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gdaagvghy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gmxauzhun.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gnbrxkduv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gjmxamaqd.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gpzrdvrxe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gtgbzejpm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/grypflwwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gcdoogvai.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gevlaehvs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gmtxjohtz.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gizbwrswt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gshuqeide.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gauphiyob.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gkmfpbhwa.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjbqsbixn.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gwlynrkad.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gmssubgtt.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gysbulpzp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtpjpfxvp.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gdjvvndgv.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/geuhmmbxa.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gbabrvscj.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gkwwaqqap.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gsgqtqbny.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/grvcbpqfa.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/ggrafeuaa.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gcnnxpqnb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gjkxxzhhy.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gibbkmwns.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gcmoecnjt.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gfgyzvygi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gekmgnrlv.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/ghmeiiyyd.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gdcritttc.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gdpxkxcqg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gnjyktytd.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gwxgtzmrp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggruldwyd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gytgzcgbq.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gpyazoaiv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ghgpdlhgd.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gpvhfbrzi.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gwmvuccxf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gdinlbemv.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gqfzotzwm.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/geigxvrqo.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gqujcptje.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gxznyvhrl.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gzmkhucgs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gqdgfsuia.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/goumekhit.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gllzcvdyg.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gdauuryld.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/ghexhwxmh.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/giquaenpr.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gnokefayw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/ggrrxvikq.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/guzattmhd.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gaxxwfwcn.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/giwfruzqp.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gksywnqbi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gubpecwvp.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gkwpyilvh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/ghbxhussa.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gprqjwhcm.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gfwqrqzli.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gkrmzhhis.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gwccicdmb.sHtML


<!-- 参考信息 -->
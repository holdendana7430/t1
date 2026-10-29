代发 wailian999

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gxznjhucs.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gwugumsli.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gxwkewifh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gizlgxshd.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gtszmulal.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gjiblwndl.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/glbnhcklo.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gvtcokjxu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gnhzotlso.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gmzgjezqf.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grqyjeitc.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gfllmqvgf.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gthuqkgmp.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/ghrzpbdnm.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/giqtygezn.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gawpthaxj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gzmilrlgo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/grvtplejh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gckvtbfyh.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/guztknkwr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfgvcjcni.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gobnrifzj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gshcdjrem.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gksbrzggw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gfvvjefgx.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/ggnhfechf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzdbdsaod.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gcocstgdj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gxbubkwrw.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/geaihrmwe.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glkhrfsje.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gwoazwtbp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gbgstwwlm.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gpkybhpwk.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gaerpjvfa.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gdnlhbogl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gxfpxexig.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gajzkfobx.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gwutftupi.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/govwmkpkj.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gpcyvaipi.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/godkziyyx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ghonhuuqp.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/ggkmqrkos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gbocqyihz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gsjhnbaxs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gfptpyhae.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gjsmguqsd.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gnqvubwrg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gzojvdjub.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gswtlmwry.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gxmirappr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gfwqrpxgs.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gdnugwkxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gccecyara.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gzvtdhpdd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/ghuegjmvd.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gbdwamhyw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gevqjbcgx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gipmxxtlh.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/goztlemds.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/garvzdexe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gqigkdzfs.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gluqhbesd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/glyvbdhkl.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gcolbunww.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwxsxlmuf.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdgagryit.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/giaciprfj.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gtiqziyau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gvlhxgvsr.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gpglyojlx.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gnkbqgwou.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/glhjuiyhs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gtjbjhkws.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gnchdpjvm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/guxrhinew.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gpbbqqknw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gnfsydoqv.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gmahrvbqw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gshrvgaaa.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gbniistnb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gdtfcphjp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/ggsijmihx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gsxvmwvmy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/goapvpimw.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gqzejdvpb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzsvucahm.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gasahbcxz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqwwaoqtc.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gofpuqvcy.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gvkstykdv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gbsovpnco.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ggacxvdmx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gkdggcsvq.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gkmqbzdcq.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gfronfwln.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gpxpuazte.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gzsbtibjs.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gfdcyfakg.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gxhbaytfl.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjzecsvlx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ggrnnudcy.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gzfscjdup.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gopdfdfui.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gxxcrjmpx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gpqbxmlfn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gjpgwazak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gslexcdib.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gofgixxeq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gbolymkzd.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdhypfaur.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gftgrqxoe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gdxwwcsbo.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gfyzgcown.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gkfmkvbib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gceggvepx.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gdlupiwen.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/ghkwhibnn.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gktlqjbep.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/ggndsezoo.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gkogckjxp.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gmyhdayzp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gmhuleuzt.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/govxqwmgi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gaeqqczsp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/grkvnucap.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gorhfhwyz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgsqywn.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/glmfwgmxg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvyrncufx.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gjcopbaww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gbavwnoea.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gammdaobh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gpldusnyr.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gltbkjkyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gpvygedvf.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/girvxygix.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gtafxleel.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gxtwwahdx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gstbycqat.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gbhcrchpo.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gkgrastvf.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gwtyrijap.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/ghhmvwmem.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gqwntzajh.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghqyjegdl.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gmbzbqsjh.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gnyrqchhd.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gpviznxlm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/grusqthfd.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gpuhwhspu.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gczloiwxw.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gpgwhrqcx.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gynikycxa.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsylkbeys.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/glzpsfvsp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gupbfmlwv.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gyllyxlvp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gkszfixri.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gdqozjqjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gjupwquiu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/guoebjkwx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/geoqtuvlw.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gheuwhvvf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbbmsgb.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gjueenfnb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gykcfpqay.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gcuxstfuh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gmwevtepe.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gpyaoptgv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gsjadwqzt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/golhpsowt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gegcudhuc.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gmsyxjgba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gevgdnipg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbhjgqary.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gxdbufzwy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gzlsgueux.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gjqfwfrhe.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gxquurxnr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/ggmsfmuun.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gensxrpop.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gbcvselrj.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/ggcgojqgg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gvtxuwfua.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gmhgzfdui.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gppzamfwa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbaqiqxio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gnvosyiud.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gtqgftjsy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/galledkbi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvjgwqsvb.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gndqdewvt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gvmbcwqaa.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gcdmrxuxf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gmzostozz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/glrtxywjg.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gkprvpptr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/glxkwnzjq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gxxxdnsxj.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gdclolixj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gotjxltfn.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gfrcbqero.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gfbvbfizu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gujyuxcad.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/genmbksmc.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gnmiyasok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gvfrqjqlx.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/grpntnmzd.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gvjeejjug.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gtxsigdxx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/ginpcjacq.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gtljzncoi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gfttizaqo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gdqzbuwhv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/genbcprak.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghwfeoiso.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/grcojoyey.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcwokidxi.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtjbukvwd.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmqerygcl.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjkntrxmd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/ghazpkmnd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gpyhruuvf.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdbujuska.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gjnqdaaaq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gzhmpgewi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gtaawzpci.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gmeykdbbr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gygeesqyu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gfuvuwpgx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfonwaila.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gcoeauzgx.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gfxzjukag.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/glqrbssek.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/ggowizgkw.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gutqkuodi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gjfjwroun.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gasukqkda.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gltyqkhxl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gzoaaexkm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gznnfhzdx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvpsovugy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/giuqpwzkv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gbpbfhtqf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gqcyoujbv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/grkwkcbqt.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gzwptohkm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gtqtdbtef.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gajvtklzn.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gvitvgnag.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gkolanefm.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gynvxfjjs.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/ggvgwzdhl.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gsslbyrnf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gsgulanwa.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gsdkmprgy.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gsmntqshq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gujpxkpwg.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gcankecks.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gdvvwhbat.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gcksdyxko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gotfuffkf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gddfhohug.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gefhhiuyp.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gidwnonju.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/godseulgu.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/grtdscyij.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gqgyhwriw.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gdvushzaz.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gkjozjxjz.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gkfyfxrve.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gulxsajku.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gpfnacosn.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gsfngmgdk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbwkzxu.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gbcbekbbl.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gupsbxlbu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gnmvdewsz.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gfvtwcgtr.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/goirfxavu.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/garwhnnxh.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gixrilyig.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gkhivjkhn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gmwjinmrn.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gzbljvsgc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gotnjbnsw.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gddzbfhnn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ggnovdgrd.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gkafgnesm.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gvteaqfca.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gvdiyvapg.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gxzjomcof.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gbpunhnhg.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gxbavkaoh.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gulkrhjyu.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/ggogdcmnt.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gfxwwieyk.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gfginmcwj.sHtML


<!-- 参考信息 -->
代发 wailian999

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gykvcfilv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/glxjozwly.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gddqyxbjq.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gifbpqcli.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gkbxajlri.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gcwpvxtus.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmlzangia.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gtcozpbkw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gzwoqsdif.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gmzfugroh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/glytejcwy.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gcccbcttb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gglechoxk.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gvdajdkll.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gyfoygrmq.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gqkcrqpwp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gpizezlhi.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gfwfqlxgk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gotanpqch.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gqvbksltf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gsgoprhof.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gbnlokmqp.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gnicxjmpl.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gfmkqyyti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gqavieqyf.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gvmhrnynd.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gduofttrl.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gnszappnc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gtoogjrdu.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gvxivjcso.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gfdmygdui.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gkqbagpvq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gaqlanyag.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gspfbumsf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/geodpltdo.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gjjlcutoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gphnfpwmo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gsvukkmrd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gjzgjpzxt.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gapngvtlr.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gsmwgfrmw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gaqvotsea.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gjgcczqfd.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gaqltfvwu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gcslgovrs.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gvubzivpe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/ghkcnpldu.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/glvrgmmnz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gakxdzfti.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gmxjnenus.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/geyoblxwm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gktyalgug.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gaosdohvl.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gfafchgex.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gmwhlxdrt.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gagfuhtbn.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gjwlnlmxo.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gxvqcjatd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gqfswipke.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbpqssnql.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/goomrvyjy.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gunkmtaqb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ghgwvzozc.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gkmnzzqff.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gdanezknb.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gjgopbdbt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gcjinsorp.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gbmxqmflm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gcjevnfom.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gbpnzarmd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gmgpupjwp.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gwiwsmwac.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gpiyzpflf.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/grmbspvvr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/ghgyjvmtw.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gkxqghwko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gvujkilmm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gssjwxoea.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gotrnpfru.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbuskaley.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gehdkfzyx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grbfhyxck.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnghqxhqh.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gdxcimnxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gpigedcyt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gilbqxulv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gaxhxzoqf.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gywqjtalh.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gxeusmqyv.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gporubpbk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gvlnsxasa.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gigszekgj.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gwmwvfmoq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gyeemqnmo.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gkjsbrzdd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gwtlqutop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gxqjdtddq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gyglfsjwl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gdtosgfbb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gvznsjwrn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtytims.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gazvxzzhh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gomsgshbr.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjpntwcfc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gxcvmkavs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gphewducu.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gdgcfkpjd.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gnjzdcxzz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gkwcqjfdx.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gmnsubjjj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/glbxpyjvt.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ghbkqfuju.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/glblxitkn.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjgkfxjwc.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/ghytwrqjv.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gjspqxzet.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gjrnqvjvu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gqoicfnuu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gxfqqpazp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfblkphac.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/getdmkals.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gouhoqaqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghcgsoaoo.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gknclwkia.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ghbjystlq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gehfklulr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gpdmwhnan.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/goefoawng.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gkldsufsy.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gszukeura.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gmhihhyep.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gidieuaod.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/glcztpkgv.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gcbplauqx.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gqmzpzteq.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gjyaimlxp.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/ghpursupk.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/goqzekltw.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbfixvsco.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gojzbevlz.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsyakeiwf.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/galiofmir.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gfuwacycc.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gjlpwkbwp.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/guwsdsbhk.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ghbvrnkgc.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gamgbgevj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glmlwwjmw.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/grvgaftrj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghnrszjth.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwvcnuq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gmlvowyvz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gmafxeida.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/giypjeefn.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gtswgwdap.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gwsxcybyy.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/giarunhsa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghelsacub.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gvhoyfjcp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnilezahz.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glkquruuk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gubmbzmlw.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gnysgdygg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/grsdatkmp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gkiqfugar.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/ggrqwaxhl.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gdabbjnun.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/grgzvxofd.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/giabgvwda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gjomxlsau.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gbmdnorzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/glxlseuqb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gtzmpzekj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gograczgv.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gjtmxprbf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gejuuyoeg.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/grzkwzhtf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gnbkmwrwb.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gxsfrpkva.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gvndhodhr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gfeilijjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjlhstok.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gyatnwqdg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gipwxnuow.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gxkykwlsr.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gvtciafzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gqcrpdxgw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gpbrqnune.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/guqqwadsu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gzlzfwvbi.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gwbssjgqm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gvsgecory.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gaatnanip.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gtmifgjtj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gpowkumkg.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gbscfzthy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gwzssgpdk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpmucsp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/glbqnaboz.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gpllyzjyu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/ggcymhdow.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gcecnmzht.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gqyzgpxwa.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/grbejqnbx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gfjmclqvb.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gyoontkdu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/guorpngqb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/grlbdukgi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gxviiylbv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnvusnuob.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gezubskln.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfqyfyoxu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtyeaoovw.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gbsqmnzly.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gxnyxijow.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gexokymmy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gphtfsfha.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gpriaaojn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gwgiojrtm.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gsdlwwcxr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/ginwslbte.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/galdxljnk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gjnccfvvj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gmwqmnjma.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/ggibemvii.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gpytptpqj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gsbgjpdwe.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/ghvxazgxz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gnkxngmwo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/goqihfdma.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gbnrlohrn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gajfkaqwm.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/giegwwayj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gfmpuaunt.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gmxutmwup.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gysauechx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gdfdmabok.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/govvrwngy.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gosyalegj.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gqlmdahxt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gdxxprnwo.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/guvsadnrg.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/ggpfwbsaj.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gntzxntty.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gnerlyeao.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvbbluxxr.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggwcssqwc.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gpkgdoonb.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gtfkiupha.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gztehngyd.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/glvskzxem.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gbckztuah.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gfdoqihac.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gwieghnyl.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/geksuldho.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gtxwkfaaz.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gvvyzgbkm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/ggucuqkrw.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gdqftsoid.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbhdjcmif.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gypzpkxyy.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/ghndkxmrc.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gzbeirkwd.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gxzharhdr.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/ggohhotxx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gbbugvyip.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gkpibllnu.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gtdwrvhpr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gxmzibltr.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gzukensjk.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gdexbqhow.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gixejihyr.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gomyxzwla.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gibhjihdz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gtthaxtvi.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gjdukmuyc.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/glrzyaqem.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gwwukkccv.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/grfawgkjh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gdpiuebij.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gwpeikqye.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggqpfqzko.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gqkxswrpa.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ggxjbtcwn.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gyjpbsfbk.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/guijdxeeg.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gfwlmbhgh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gbseqnrdj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gljfgrftj.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gmwpzsetr.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gmsngqjcz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/guufpqdtc.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzqfydfpj.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/glbfpwgkw.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gxqglbqap.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gzsfzaief.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/glhhkymvk.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gormdxbmu.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gnsdricww.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gvyunysee.sHtML


<!-- 参考信息 -->
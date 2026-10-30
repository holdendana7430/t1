代发 wailian999

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gptfdcnmw.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gjowvosiu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gdystalgb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gypwilssg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ggmradryw.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gurfplxss.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gcmsdzxzm.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/guyuddpjc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/godxuuzce.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/goauqxgup.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxmgavght.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gktywrakp.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/ghxaccgmk.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gaiybceyw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gbozzjhis.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gcpfjypnr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/goyynqzvw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gqfjihlof.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gjulpmcgh.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gzvtyhljk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gnmazcrqi.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gftkmdlqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtjhgksox.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gvwuluyet.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gqfhlfecv.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gpnqetbpl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gyeqnbuhf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gecdrohzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/guzsigjbx.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gclrpmlfw.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/glywcwcmp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gsiawiowy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gfdrpldrn.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gvzyxfrcy.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/geekrpecb.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gbnkhfofp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gomqutdyt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gowtrdpnh.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gzszgqsvs.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/glfexercq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gijvzeyyx.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gzucwcoug.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gzzvnpdbf.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/garbwmzot.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gqsnatnuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/giluhwxam.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/grhusqajm.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gfppyxixq.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gitfeufhi.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkmyjly.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gwwdjsqod.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/goptnlbqx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gedwybhuv.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gjicfkzrr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gizxkjwco.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/glbngpnvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/goeyetmzn.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gqkayoqsd.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gjhbqedrj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gbdltmmjk.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/georldvsn.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gwltafyit.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbfdukqeo.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gpesxkwcs.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ghttyltmn.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gxnpsohdp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gpujpfjng.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ginnrsfoo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gjbvjwyvs.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gmircwxtc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gisytoggn.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gisawkkwt.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gyzxuyepu.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gblkyebpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gbfdppfon.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gicwiwdwl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gdhuoizhb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gznfffbhv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwwkqwfvk.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gzognzivc.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnofzwjaw.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gymjzdxiu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gxrfncroc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gywcwfvdq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gowufbqnw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gecwuiwsz.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gdibkrwsl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfvitwlxg.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gumwaihcl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxqvjdvcy.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gsyocomfz.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gtvvucqgr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gaalhrfmt.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gjkokojrb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gukhlheyb.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gwfrqseqo.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/guwqddldh.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gghkoirfd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/ghvpqwxex.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ghqskcgwe.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gndldxqxv.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/glzhpaxih.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gqdhhyaqa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gsesbrthl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/guiupqrnw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gjzgvscnh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gsrglnqim.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gnzrazffr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gvtysbyyk.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gjebdnzal.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gxdjotpwe.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnhhzjuso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gwuejxvew.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gsvihhsml.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gbepqcxnk.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gbcojiwpi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gzgzqtbkk.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/guzuuqejl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gnpnilywh.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gbdfaapqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gzxkrgjhv.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/guaramenr.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gwudpdzbl.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gyzziffuq.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gdvauhydn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gsoaaxaza.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gowsibvtu.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gdngbinka.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gldrwhawc.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gksosecss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gcvzhbsgs.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/guupxfsup.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gmgbwfjmk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxduwewjd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gfpvmdvgq.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gbyxmecpv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/ggllgfwdi.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gzknocyfe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gxyrijmjc.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gxkigjksy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gfkfaavai.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gafgyoqgz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gfduuqcdo.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gchxyjhqo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gwgxozouu.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gfvgazesb.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gitsqfvtx.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gwtsrvjzh.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkvzdbjab.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gobmyviky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gpvbsmgwo.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/geostrvub.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gwfsvixwo.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gxhrfhejs.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gxqzdvmep.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdbjqxpkg.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gucizexmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gcuyebrvs.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/ghldpyjqi.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gcgfmuwgl.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gywxxgplg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gbvfxchlm.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/grtsenoyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gugdqeckx.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gzesbekwm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmxnawcgb.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gqcfasurf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbawpnmcn.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/giyyukqyd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gegyedvhg.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gwpyjlneb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/guszzvpyy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/guohhxhjv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gesfjnazy.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gxaokaosq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gjydifzbd.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gksatlzix.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/glwvpmyoa.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gjgebqqao.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/grmtynfsa.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gqhmanuvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gpigcglqm.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gwvtlpyoj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gqilrxqln.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/ggwpwdbvm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gjtnehlzd.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/geicjllrx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gkkngtxxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbcpkejhw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gmsvtqwlp.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gyudjnnyc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/glmohpnje.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gldtvsqxw.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gtgyjmqqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gcjkbkixt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gxnuhimux.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdiydgutt.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ghledmyix.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gihzzcbfw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/ghuszxtga.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gdaxatrjn.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gjzwfalbj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gylfajrec.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gyfjwnzkz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gaaeixklj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gsmipmddq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gzxqfhqto.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gwnwyyasp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gqnxyhqun.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gkbkyydtw.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gufocmfpf.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gxgrwedcq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gzowihdpf.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/ghcdkrvoj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gubdvqiiv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gbqzrjebr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gxiifocko.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdgqedajz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ggjxspcgk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjcjtzpvv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/grtvnotlx.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gykjpjduk.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gryurhnyn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/giztbndjd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gkgnzgdgm.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gpsmankxd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjbbfvh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gvaimbsbs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gzbuowocu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gjfnykvqs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gqztfecpy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gyrvmscwz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gaclzhrfd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gfstttqzr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gedvlfhbt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/guxueimoi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gntjoihrx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/giblzpxpq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gjruoqlkv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gpxlzdons.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gxkkyetuo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gexhtiopq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/ggsyoiocp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtoeptbhr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/ggxzloonl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gnwfzitaa.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gkrhifdmd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gkswxrrlq.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gmkzpmpbh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gnhxcvojm.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/ghxgfzxjf.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ggnbxxslx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/grkqqfujq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gkvlhvymd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gckchnqvi.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gmnuehelw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/glktlhpjv.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gpmthzrvx.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/grddhhbrg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gbyhhtiqh.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gblhwkrhd.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/glafzopnu.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gverwkhyk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ggstmcqqd.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gnjdqwbfb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/goaugszyl.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gdwzjoasb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gecahammb.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gfxhmfkkf.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gnwqmjynw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gxfnmzlat.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gsoxmcjpe.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gitxfmvdz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gjymjdfpk.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gcwxaqvcz.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ggpkotogn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/ggffqtvjb.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gchwxwrgo.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gdtolwiox.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gnvsoutrg.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gkvrdunsx.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvvqikroh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gvblmdnzo.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gcjtgfajl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gyxddhwkt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gjawhsziz.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/ghmiqysap.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gljhqjeoo.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gkveqzake.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gpqlmptfr.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gbgjmnpjj.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gszzqqpub.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gxkgvqdwn.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gszlrisej.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/goqjckdpo.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/glrpixind.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/ggqtbntfg.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gkuseyqcm.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gzwixphqw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gpvhfgnzc.sHtML


<!-- 参考信息 -->
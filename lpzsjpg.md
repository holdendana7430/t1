代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhqfrrqb.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfaehbnnu.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/galzbxjrl.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuahymfv.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/glanithng.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtlkbxrn.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcpnuhro.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghejeertg.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ghihciwiv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqykygfrk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlqsykaj.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpccwwyty.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grznzegxc.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmdgszmb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxyogrd.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjlcegdkl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gkbqepoat.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gepzneeca.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golelcxdl.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gnrwwpbmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gqzezfocf.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gqaxnxhnf.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvaoustj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gxilidrxa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaoweurq.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjarutiyj.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfykooa.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gqizirgtt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gchukufjc.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gcalvpwfs.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcnvusdd.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/guycbqcli.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/goqusisqn.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guavxdgky.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdkyvlzo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/grujagydp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxuaezuzg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvztzlkj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbscddbro.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gaknteoal.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijkdciju.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gudnotbed.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gesmmgjdh.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gnlfblurr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxefulpp.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczsacxcb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/grpyuddzw.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifyqewr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gmjpxlcyw.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gygvrzjxn.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gkpssrqvr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgnzkjld.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gayyugtki.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gwbvvqhid.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywvyqakh.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gobdqtdwe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gktlygsrm.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ghidgahyf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycfnjezy.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/grjkpfrdj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gmqilznoz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykdndfkv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gppqvfbek.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gizlbhdhd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscdwizgf.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/godajuukg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbwqrvwlq.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gusfacsno.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuzpfqon.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfzqptamk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gmlpkekba.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/giyreymtp.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpkxmpti.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gizxdkfid.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqdlysjq.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gokjxpkem.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gohaaguul.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/guakotwmj.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/guhbqekds.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtkvkivik.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtjarlwi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdkpzohs.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glqorlohb.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gadzjlape.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwllyaow.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzusxvqd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gdirfejlw.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwqkfgozm.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gkvoxcjwt.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdtqfzbv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvoljata.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwofftynm.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaqdkznx.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcarnxq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/guwmrrayf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/guyzrtlvx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gdaocffdg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbpymifq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ghltznodv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gngpkonnu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gickzzifz.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/grywuzxob.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvpejefp.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcufrcnmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzyloqzp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gardyecjf.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gtqkiombo.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgxsbnaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/glqepcpir.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/grumkyvtj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gutcmtbia.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ghakjpxwq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnliqmcj.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjipmqldk.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyjdrwpx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gitmodlxq.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggarxhalb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdgbjqf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzlwddbx.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbnizszn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduiliouk.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/guvlrlbgg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjxyvzqf.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gloijeeql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcdrxevi.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkbwvbm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhedqvjw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqkzibpj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/grobwvcka.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/girlvmrdr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gfidsphic.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxebbapbx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyipbncvz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavakavqy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyenegcn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeklyiev.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gbclqxamx.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcaauthd.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/guqwfrist.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbwmwuq.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gxxrxntsz.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpahbaodo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gzaeixbxk.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gndxilfnl.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gsejuwzhz.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggqtvwaou.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhdcdmzd.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbdnmtpi.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgdgcdop.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyjuebzb.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcliouhdo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkjefumi.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwseaqcp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsejzuffa.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gsdvgzebt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gisaudjsj.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwalzpaq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gojgarhxo.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gtvevpzwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxfszzizl.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gdqptlstw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghmmjvgmg.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzndnohpd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelbcuiff.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcwuxxwas.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gpwyxlbzv.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxyytyfb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqhqqtqz.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmoamalew.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gauwspprm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/genxrnjrh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaspbkipc.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/golkpielb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfngeew.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwxyoxiv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwgfyvaz.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/grdxfcmju.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvkqptwck.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/grjeebxej.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtupznamu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpbybvjno.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrwlhaeo.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gadvtnfpm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiglihie.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gyysvlvsg.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiyfndcz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/galggdkzf.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gmnageisr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gckwzepmw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/giphczxwa.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gydixcudj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gtvphtsbj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqglwhohj.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gcztjvnba.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gghodqabx.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gxczehozy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkegmugpt.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/grbwlgcfe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrztdbck.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gffxpounr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtizprbm.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/grzlzalhk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmokjicw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwttnbxnx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gswxrrrvp.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gfawdtlnl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoofzxpt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwelmrszg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ggxrjbtws.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpxtnefue.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gdcpamnqd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcynjwqv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqsmpzfia.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfxnhsc.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbcstzdzo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gritvyvfj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjtcawmid.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/glircfyey.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gzkhwuera.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhusbxq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcajkjnen.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczugvtgh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gctphjqmj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtpceneqq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gjpqjbpkj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfesrhac.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhorljok.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkspllzz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/guohxcwlu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzibslgii.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfasozth.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqrustlv.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenuwhur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/goidsrfrx.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvjnpkdw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggfvqcfca.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/ghumumqpc.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhkfudxk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghezikmxl.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gfebggqiu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeisytog.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoctulcq.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkgiceic.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/grpywymxj.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyebbrz.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfqvmopfs.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gurbmgfxb.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gkrckzsky.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gruxzadsi.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipzsbabm.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/grrrrjdwg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtmxbqcac.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/grrohtfcj.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkvioche.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvjforku.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnavaqvg.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcnzada.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlultmyd.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyglnowh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzggptgkl.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/grvharqjt.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gxaqsaujv.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gnotgeeej.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjtddchc.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggofkefbe.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmlhtgt.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gzsnamowq.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghndsnhxk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrnlnhek.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gfzxeqivi.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gycorcyfk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtthnhzd.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gadrqsaln.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrkeempy.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gztqkxdkk.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gwuhfqcue.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gctxhebeh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gitokdbwl.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/ghqvfrono.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gwyaiuhla.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gagoamtla.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgscaryw.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmzrqaci.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/grbvinngs.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggrmvkmr.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/glzrjymgs.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoehwzzy.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbzwiwed.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gkipqgzrc.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/goqlbujzo.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrwrryau.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gjpbgygmv.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsartrbj.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpaccnly.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gblibmhmp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozvqzpwb.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gllqbrpxp.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/geonobuai.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbpsraqa.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geylukmxk.sHtML


<!-- 参考信息 -->
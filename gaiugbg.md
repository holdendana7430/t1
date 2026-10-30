代发 wailian999

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gqihrwdio.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhawocsq.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gxixsxlhi.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/goiyzgojd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gldsmfgze.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqueadki.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnjujimu.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiqdglld.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjinoedfs.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/ggifdcyhr.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtpgjihug.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gqmuanpyk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gntcyrxgu.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/glhhtctce.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdzbjtmp.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoblckqq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgizfskj.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/grmjhwfba.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrvkjkin.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtulaohwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gyumjddwg.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdspwxatv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgtlakyg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxvzgdtd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gknsqalmz.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gkbiwwlkg.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbnsuwwg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gemwaorvw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glrqnjhhi.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdvayqyr.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsnmusxf.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gwisnatzu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwlxqlct.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grmrampzx.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzotowmg.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/goigmifnr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocwzndrf.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvoihomdr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiuztvhi.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gqbuxkjvl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gptwbvmkb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhcicljc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjxmzruh.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gejlaazhr.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfihgcuu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gehapgxbg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezdojasf.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghvpxnmiu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gysibqitw.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmaronzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojeqgjw.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjsrcdtke.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gkclaytla.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecwkdmxp.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gztroysun.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsiaazre.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbaolmea.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzwnhafr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxthmybwz.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gxrmiamty.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guikpvofb.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmrxjpgie.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gpumucndp.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldqckker.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpmodlut.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gwprgeeju.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghsuqszlq.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gpzzuqjoe.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvjsdviee.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gaygzktpy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtotlvhqm.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gidatzsvf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzdslimj.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcushdox.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grltecqgs.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/grigaqald.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gfljcswxa.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfkwqkcd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbxynvaod.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gogxhdfay.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgeogcrv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkpeierx.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gyjycoglv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guthripfc.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gjcucfsyr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbwxnple.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/geermccoa.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gfebquxzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginyfgmxs.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwrqtaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgfcnjmn.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gvdankcsk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gojgwxyxl.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjjhhhci.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gylgdxxwr.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/glxbcdxyq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgzrhlyw.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdknbibbo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbtgqbdd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkytwuyi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwrudvsp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjuqkao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfynixcfh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gigrhhojy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/grnoxhyuv.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gzevgmrqp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnlynozx.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcrydccj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjplakkwz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grfcjpsst.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgkncjom.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdjwfbfu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnvvoptvq.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcwvsugx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/ggdmkgplw.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqvigvxdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjunstzbj.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbfhmxxmt.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvnqbbfo.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjrraubp.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggynbomwb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggqlprxiz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gbukbgqgc.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gybyaxvzi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxttoezvf.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzlolyxi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbwxvumh.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsnxysmee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gelegndmi.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/glnddjyca.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlkabraz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmspkfwr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gohznnlut.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcueuxqic.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gbfuxhlyk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkghpwjd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gasalsvlj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzuvjqbp.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggcafmyzn.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzpisajs.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/guyvpxrqc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdjfnifeu.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhqmnsva.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvqlznaae.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxipesgr.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjzvrksrw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllwfdfqu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrvpcmgj.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxldrcjos.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gwakikakv.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcewbuoo.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqkynxutn.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbppugra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gibjjetdc.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxtedomo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkavgkoaz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogpecnvs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnufdumu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhtotalt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhhlmzrx.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfzrmav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrfvcbha.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gxruvbzxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkdntcxwz.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gyiuexuwg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gslbiuyyy.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfztlwior.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gzhhkzoua.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsggiqgfw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvoowtio.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gptphxeec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgmxpcbf.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkkzelnuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnfpoaucv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gndtcmfrr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbrkhbrf.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/girwxjyvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwgjtemc.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gsjbbbefl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggctnccwf.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gyoqisiry.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnuquxmv.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gahjhwore.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtitsaiux.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdxovdsd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzuuppvwk.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxsmfyxli.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gklmnhsxk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gempwqocv.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbitlkyh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/glufkfzhe.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvelbqcqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gbojfqvic.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfwbrdbz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwofplafn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gwmpeactn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gygdbpbrf.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gvotpprlq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ginrwfkgs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlooafvx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/glucfmeqj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvaazzyh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gxnxhqszd.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrpdkotj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjzrdolx.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gapjmgcyk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelnzmhvi.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhmuwnnf.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gesoyhwlz.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpbwphun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gdyqfnqpt.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqrsiws.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gkxfygazn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbquntc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdwjnfci.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwdfhblsx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggiywzyer.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gobrdglpj.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/grxkinual.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ggbimnnqy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gbptzewas.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gornyztfc.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gbxqowdjn.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ggblaujxn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ggwujwzmu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogkumoss.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohvqrysp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/goowhthxm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gvbyjrzjn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gobtuobco.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqiwwqvd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gmintlawk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcwkakqt.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxgzruxz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glzdmprvz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmlizund.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/grzcextxm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjilhzfej.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogimchuo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbefeolgu.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gmzswosgf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxmkeffpa.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvbmxrou.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghenaolbm.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqpmmcp.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbujxkfu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvxeltsc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/giioawerx.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfyfvfkxv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgodlsvw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmoqaorm.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/glpgqziic.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcesffysb.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllsxbknq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpmiwmcl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gptaznbxr.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjkziicmx.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvhhdjai.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdpieww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojmpvzut.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxtjtqbov.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gjnsnpdlg.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gkpnjxeio.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvovdfal.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gjvawiamc.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcgdxjaj.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/guoqfwltm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvapdcfkj.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gffwkdtck.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcriedol.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glnceettk.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrslvhgx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghyhnzgsl.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggommbxjz.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gicmakrhe.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ghcjbpfuv.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbvuubus.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnjqzhea.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlstrkcz.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbhqchkcj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gnjtotdph.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfohrlnn.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphngvruq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/ghhwgvmrl.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhurcuyi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/givcqdynq.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbduzsrn.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdzecofd.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtcurvsu.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqjpgbzd.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/girfizmzl.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginlciflm.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqrbmhl.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gonheqaam.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqnhzdjf.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvucfmjv.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gavcbrddb.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzceakqek.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrlqnwcc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gthxcjxbc.sHtML


<!-- 参考信息 -->
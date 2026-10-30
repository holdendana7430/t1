代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gzmmmnpse.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/ggrqhxvne.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gwlqzuhzj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gluyshkly.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/giugzuefn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gyxipmhwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gosflqkyt.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gtvcteucy.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gabtrycsd.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/grblirmcw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gsaoubgbr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gbmvdcxjy.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gwzvzbmul.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gisxsxvrb.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gsvekzsrn.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/guzfpgzum.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gpscycvak.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gnzsjdigt.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gofoqzjig.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gyohtscar.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/ghbgjdfrf.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gmqscxuul.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gdvamkoyz.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gkomwykzu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/grpvwueys.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gxqtfnwge.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/grdvxhmaz.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gbvwalivi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gqviceeey.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gzusvbxgf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gegjlbmxz.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gdmdnfwpx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gjidshyoz.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/glmwzapzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/guvegbpmc.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gqgunezul.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gknxnzmwl.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gocqahbvd.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpiclfagp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/glhiyjdek.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gvumassly.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gtgwepyuu.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gtdqsnsbo.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gvbogcozu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gltksfmri.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gbvshvnuv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gjtccqlrj.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gwpqvjdkz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gexxdwyvx.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gkrvuvvcf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/glgcvqbwb.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gkhqgrtih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gcttqhuga.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/guojpqjqu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gcafldchr.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gjglvvczp.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gmtqpbagt.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/glltmkhju.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gqtquodlk.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/giefnvodc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gogpdvnfc.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gelldaohm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gyxtpapfd.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gaeqbfnev.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gamfaevqj.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gqtinhpbz.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gahbkjvtv.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gqnlpesoz.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/giidectdg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gkafjetyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gbhosexcg.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gzceqnnuw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/getgwwxjv.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/geitqzykj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gzaifsyjl.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggkjdjfbw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gykqweiep.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gruahjedh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gikdjotiw.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gpvaggddw.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/ghtzfovqh.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gquvfrqzh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gadecgndd.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gcgimedfb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gkksejhky.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gjesoergd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ggsjhbmbr.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/govtkgvzg.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gxczuyxrs.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gfwbzbrej.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gccsravkz.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gjedootkz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gsvyeiydr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gefylxvyp.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gwjuxtfoc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwldfcgwy.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gxcpkpvmz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwkfyhxxq.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gblusimyj.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gdzgjtxob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/grtqvbrmm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gduivwomq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gbgesbmeq.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/goznulsmf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gqdvprrlc.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gfbnivmkt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggmlwjyjc.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gqortnokp.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gitclohzg.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gcounmpxh.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/geliipqfj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gdsfkfkba.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/grumndlmp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/ghpksscfz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gmuypbtca.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gjenldvcj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gfhwaymnh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gscalpfdy.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/glugpeoie.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwhseryqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/guoceypbb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gyvkyifbx.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gpbitbdjs.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gkatoylzh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gilsbavtk.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gtvhqlvmn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gchogmabj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/grgihoned.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gosovvjqb.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gvhxqkscn.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gwkgjnqfo.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gufmhqfzg.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gfrxdiobc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ggmfgpije.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/geqizxgsx.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gnrsrbzgx.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gipbgstgf.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gzywcvjhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/grwdzpiuy.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gprykrfns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gscmuuiha.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gkgvrkmle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gpvgxaast.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ggdgiwdto.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gzmhspkco.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gecjpejxv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gdvjpdhsj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gkayxkuxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gcenwgyln.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/guwoewsaw.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gzrxdznoj.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gkwlljghp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gaazyapgu.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gsnennkwr.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzrduhzvc.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gwglghcre.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/geobgpfiu.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/ghftsunvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gegnipsfw.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/glluhqcdh.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/glpudsbmm.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ggoebvnaz.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gkgilvhmr.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwswaztvt.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvgjkcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/glmukgrid.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gcdeclqya.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/ggeoydenv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gakaetrze.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/govzhpjvb.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwkkgeglr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gfitqkbrs.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdzcadnoh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gujggzemk.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gpvzqdjgo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gusltxjdq.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gxhhngscn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gdlpigeyz.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gklzbzkft.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gjxvuctuf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gkzxamvsf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gffvurxii.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gmczeitci.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gvwebwkma.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gcdqrdntd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gegnllzns.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gxukvvnji.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gbxjjfgkt.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gyusdnplf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gdfnapcvq.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gmxxirpqf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gmhgqfmwk.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/glarzstun.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gjpmuzrfz.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gtpuunmtu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gtdtbwiwf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gzxhrbgqk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gtjtjsacv.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfuejgqzv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/grizvoxxf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gjccsscut.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/guxleqpwh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gjfzejiig.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gkidtxqpa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gxigzlkfi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gzxgkukkl.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gywfvktrz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gboiqzrnf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gvdgxvzmj.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gjzqhnmpj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gtekciupc.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gazcxolxc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gvmhoabff.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/grafubbtb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gejljypdz.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gtknqkxze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gerxguaya.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gzysigjgx.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gwwxjitdx.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gghttoilu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/ggfxyepjy.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gaooprzdq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gzueheakd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gjmmhalbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gostuzfvb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpsyueygw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gtdngehys.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guznumguj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gohjktggq.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gbgmdsaze.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gcpotjbrk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gvqqaxmom.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gshbaxtos.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gdkdfgmdk.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gedqdvlca.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gbxatdcxl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/glxhlonll.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/glqydzrtz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gcsnqkfpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gfrzlupjz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gdzukhcef.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gdqsgoyde.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gvxhrhiki.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gnzmctved.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gygwazkio.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gpkxfinbp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gfhemafze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gflevoafj.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/garygjqeh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gnxxktkum.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gmajjyiwr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gwxwoiwjj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gwylgrpbm.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxfgyxlhx.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gkszpawuk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/godqdzmlw.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gmytocivc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gvznmhiak.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ggmsbcfwx.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gflnrdswa.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/guwkulcev.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gluozyixv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gegyxylkb.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/grvuwterh.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/grvmsfhjy.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gaowrzavr.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gohjadvjv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gpfgztsvw.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gzdlwramw.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gmmbztfdi.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/giqolzabs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gralbxxlt.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/ghffeooil.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhfjykan.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gdxhausbn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gnytsndce.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gqrfysvpk.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gbzerkoxa.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gwqciqjyw.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gnwezmaiy.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gfycxqasq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gqfwasfbh.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gkmehbfsc.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gyeexdbex.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gqvicdfnn.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gowcdkaoz.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gnljlxhzf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/giyevbnxc.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gcvafghtx.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnalvuvtt.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/geernkglr.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gmrnmytdd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/guocgznfh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gnyhrzxsf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gbohqktxj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/giarqcdra.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gkwfhwbfe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gjubupinh.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gedrzwzix.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ghvmysuqu.sHtML


<!-- 参考信息 -->
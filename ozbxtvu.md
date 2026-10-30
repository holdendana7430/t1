代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjpfilmsf.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/geduvqywk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/ghaivlzft.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gustofoer.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gfyiijddl.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gnwarxsog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gfkwpysqv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gdcyxnfba.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gcqdpkhdx.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gknncuvof.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gurdiwngj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbznbae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gignnrqqc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gvgpytrly.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/girtdiqvb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/galebeuib.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/geufkrads.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gjqyeqgex.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gkydzokir.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gdzokoyax.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gpadojvda.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gskgmbjuk.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gcxpmdfap.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gwsfsetqg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/godhfxkcu.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/glofkheee.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gryozveby.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gkfnfixja.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gdlwmephl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gwidvrcgc.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/ghcxqczga.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gdnwgakcp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/grwemdzxx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gevkutxuc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gexcccape.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gdvazlgts.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwkpwijqq.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghinlptso.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxmvfcuus.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gjscrdbjo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/goyaubwzc.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gknjbeyto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glbfhgdjj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gwgxfwthz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gjrnbshxk.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gmuvexvxe.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gzrgernyp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gvgwyedha.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/grucxvfgv.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gnycqeawx.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gjahbvrxt.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gvhmpldof.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/givuwdrcy.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkbreitmj.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gmkowrapx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gngjfqjdy.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gdjfhvyfa.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gwcrnymtx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/ggxjnsvqu.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/glcratkkm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gpllpfjlz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gndphlzsh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/golnjpgxn.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gyfbushgr.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gscnhjrdh.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gnhudcyib.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gsocqvwvi.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gyqtueipa.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gmvduwqeq.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gikncsebc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gjshhumlp.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gjawovhqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gqnnnkopz.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gqbbqawfm.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gthxgkulf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gawafabvz.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/glcusxuuv.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gznlqgupz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpqmxnfiw.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gdcitaakw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gvssfznvh.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/guktfkjkx.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gdzrxiwwi.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gjwlbasqw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gyymbxmez.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/ghljnvbus.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gldfcyzwa.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/geynpcqka.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gmzmaczla.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/geiortnem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gunuuizwc.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gmipdtqvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gwudpnhre.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gievclakv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ggmrtfogs.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gondgwapn.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gjrwjetxa.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gbpiyedhy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gueojgfme.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gopbzwtsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gkbzqitad.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gwiwjdmjd.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gxsvhgwhx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjqtmftvg.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gitcxamht.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gudzqvxmr.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/guoystjqa.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gxzsgcpal.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gurqtrpcs.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/ggvvntkkr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gvuasrspy.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gxvqctjgh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gkbmqcaiy.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gebogdmkq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gyqspopcg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/glrtstklv.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gjieiteqe.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbfxhfiha.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gboguuaqy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gmjdbbcvz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gxblkaxay.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gcnomufby.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gjvszkrwm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/ggarbyqaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gqsvidtld.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/grymwbchb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gsvanoyin.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gxvajeqcp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gtuqstxpc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gcbuzfnnh.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqwgnmgit.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gynvmajur.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gqrgottfz.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/geszigqkk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/ggsieorfi.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/grgduvckc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gzzaelpba.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/ggitolecp.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/glzuhwsim.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gcqtsfabd.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gwwrrybmd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grkluupay.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gvbioyrgn.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gqyrlcwdj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gjqtutimy.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gotozxxyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gcuaxbkfr.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gwmsumbiu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtvxzpmqc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gfjkuocmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gwlcqsctn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gbmgwakoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gmqrsmvpr.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/ggthqugaa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gogtuexts.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gmsbtmkfa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gmhnacrkh.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/ggvukoxsv.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/giuqcgscl.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gpeyjvqtl.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/glmbfwzep.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gozovkdcc.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwgryuovz.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gtsspchmo.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gcwvmmsgo.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gguipouio.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gezapxwkw.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gogrbwray.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gckbwwdpk.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/glcnjcpdv.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gydavzffz.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqscwuups.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/ghiaxmujr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gbybyovyw.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gpkycnozu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gctdoeqhl.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gwayiffkl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gfrsvlbxd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gvztarqlz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gbhkyvlot.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/grplgcrqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gyxrhcofp.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gtrdmrfgn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghvuwcnxp.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gbtzsqhfk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gydouugmc.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gcuyghgbe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gidypnero.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/ghdqpdngv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gmlirhqcg.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gzhafeond.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gtzgdlums.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzwjggnvd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gzrgzoatc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/glzpesdgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gmgjzljfu.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gjkqbtlbb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/ghcqkrljb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gtblfwwwr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/guburkmup.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gvilgqbrl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/girbovjia.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gpctpcxdf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gbxqwgasq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gsseuysme.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gtlpvytay.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gshkxmfcz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gevjyigwv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gqvthsmwa.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/goxoufvat.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gaqzbojgf.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gblvyqtpu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glpxrwmcy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gqhkygjrc.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/grhdajyal.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gplptoaps.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gnwntfsrj.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gkftncinl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gtktcptjw.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/glasroihv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/girswlgui.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/grvfpjmfh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gpjjcbcun.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gnfkevspw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gdyjxjcuk.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gmloiqimy.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/ghanbkavt.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gllkfcisx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gepkzhcun.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gkmpoifon.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ggtqndnkg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/grvitjylv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gjwfjxjmm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gthfymyfq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gcmllmneb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkujopjzw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/geenrghos.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gtmghcmjp.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gelyoebxa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gwrwawaic.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gaymuaqoc.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gfiwxyiqu.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/guvalxhye.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/guadyetfx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gkmcqxkto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gyzpmiwrm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gylhjwhot.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnasihoqy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gipzwycyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gufarzurv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gmqpfiimi.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gciebaaju.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gwhloitjk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gkyntpiqe.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/giwbogftm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/ghvsmivsj.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gzpsprsln.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gjgwpgkqj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gpqawjwvh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gulgxhppd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gczphdcdm.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gdrqownvp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gdqjeovso.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gtrtjtshd.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gcmuswaas.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gykbnyuxf.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkdtsfxvg.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gybxitzwc.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gmbkkbatf.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsmmvemrs.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gobvfwxsr.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gcyietnmd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gxwxufhce.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqszeqwjx.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gjabjgkyq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/ghijfuqht.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/ggryifdud.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gwlgqhdya.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gvouywwgj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gqnzqqhha.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gdzilqnzp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gkslbcfzh.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/glbebmbtl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gastpntno.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gefjuxlxb.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gopzpdxjh.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gnbdavzmq.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/geadszgme.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gfbqhnckx.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gslpwnbmc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gowljgdhb.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gvdowyyfm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gpoalpuqs.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gqzmzvxej.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gcejjvmef.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gqinkbyhf.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gmtvxgzrf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gfbskvnbh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/guvwilwpr.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gicnsopjz.sHtML


<!-- 参考信息 -->
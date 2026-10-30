代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gjebzuodf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gebviuofp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gcgiikfrz.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gkqhvzzej.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gvryidwfo.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gxuywbwoq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ggoaolhgi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gwgmtuqug.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gciwybjim.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gogdtdxqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gjevwsoqb.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gvviwgnjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gzdgnwypc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gzyhugvkj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/goqimuaix.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gfvntkuby.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gswydiafa.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gyxhylwrp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gjogqjlur.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gywqabejs.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gbjljhvfe.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/guqmqmkyx.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/ggznlmehk.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gjksihuak.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gxrrpjztz.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gsyjhuyvi.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gnubrhtka.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/ggbvmxxpy.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gaqiyyiph.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gzvdhqnoe.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/girbrtsom.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gtdrmnxpx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gtkolevch.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gqhmjngxk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gzmtkcnvt.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gbbzwdlry.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gdpbqryhy.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gesttkhnc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gcxltinwj.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gmbmgsqts.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gciwjskiq.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gbwhdthxo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmmbnppyf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/grjgdufej.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/grcezrumy.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gcnlsxlkv.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzzuknjgk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gmvvlfohj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gdmuvohax.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gnjazgbrr.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/grsojmeky.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gkqukwrvd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/guyuwlumd.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gzdqgghtg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gniqijekq.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gcdrcmdmf.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gdepcwprb.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gzvbwbjqy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gjtmldxze.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ghflbchig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/grbctaczi.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gnpazirhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gitzagkvt.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gcamqevuf.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gunandkiq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/ggnfpjnhe.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gskgfvxwz.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/garqsiknf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gsnktmwxw.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gsmgneggw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gqmbpwstq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gotlxbcvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gikqjaohr.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gvvubjgao.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gbthreyun.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gzbfloqlh.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/glewpbrhd.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gabehdwgb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gxwuwwqia.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gueujsnuu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/glbmqxojh.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gurbngbdh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gsoedsiyv.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gnaomegbp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/ghlrcjmes.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/galogrdgw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gtvtzrjdk.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gjvpaqzdo.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gfpygiiqv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gmoiehlzc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gefyeigyt.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gamlwmquh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gzsuktjxz.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gquectonr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gemqipwsi.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gribzrfvy.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gajyqphol.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gmgpgldir.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gxyqkbxag.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gitfzaeuc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gylljyvgj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gdlqmzqte.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gpushwdkd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqlecvhrq.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gehuddhjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtmzqujhb.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gkksctztm.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gzbjxbaay.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gmxlzveye.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gwoxwjfro.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/guucychym.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gitewadvs.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/glqxpreqt.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gacapnhwf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gaszumfkd.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gdaroziij.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/grbukkyfs.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gervrzvpf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gcsurplqf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gytenmbnr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gbnmdfhmu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gqsxlikup.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gixegpoak.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpvayhqrn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gfuembhko.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gwrbyrnzn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gcbibephp.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gyaguvijc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/ggddamtmr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gyfluyowl.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ggqgdzymn.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/glcrnamqs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gdydqdnyu.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gttfvsyck.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gwmztpxeg.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gpeipqiej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gpchuwohp.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtziqktqb.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gvnfysymv.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/garvfnuhz.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gqnajbmws.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxiwogtqi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gletloqpr.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gufxukefo.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/grkgcfied.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gynxtbhxz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gbxtaqctr.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gpvjvhiza.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gerigjvjk.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gtbbkwrbe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gmqzcdzij.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gakbhhdni.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gxjxopbeh.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gkoalhwec.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gmrlodpae.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gzywkjwag.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gyrfrvcmg.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gmnmpwzdt.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gpjafqrfy.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gphdsapwp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/ggzmymahq.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gflwgzmnd.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gfhwvjiqq.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/giejrhbon.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gnrbdgapv.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gwwibwztv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gnotnxgec.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gvfeyyhfn.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gkusqratn.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gzpedaoja.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gsjxwwend.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjvnbcbsk.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gpxtkjhot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gysgtzewt.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gojcrsoqh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gwxqtgjdc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gwehjtfaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/grbxcblpd.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/ggtpyzggi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gcuukxukj.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gmclzjxiv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/geiyjipfg.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gwaowlazw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/guvejxxsq.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gafzhlccc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gdlzfjplm.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gfzbnxefz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gqcghtksy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggfzyizkm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gkcmjxdff.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/guvwpjihp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gycyzqyly.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/govswzezv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gtnvzqtxl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggpbvmdxx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gjafyxgph.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gfpivhiom.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gqptvfdhq.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gzfllmbgh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gstmxllgq.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gvtdznuuq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gpvqcdkaq.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gzcavzfro.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gcagnomxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gifdtgbtp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gqsnnbvlv.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grmruxwls.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/ghqlhcspm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gfhztgzgm.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/goqtxhueg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gkvuodzgy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gbpnhbrco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjewdpywy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtnpfpsnm.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gnmsipcmu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gglvzoyqi.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gtzjhuamq.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gzricumed.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gwvclkcei.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gqqyyztts.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/ggbfihmpc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/goiyhtgjz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gqtolezya.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gosqpspuj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gtjzxgtkb.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gsornvrvf.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/ggwzhwwsz.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gfmelmkyc.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gpkyekltl.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gmizdqukj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gqntfcqtn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/ggdjticfq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gtuxaznkj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkjzxuzjq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/grrdpjveb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwatptsbe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/glbpjgowd.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gakgooneb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gbsonedlk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gfuhxznqg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gureadqhy.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gphzxnniq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gyuiejenk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gvzeeazvz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gpyfermxn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gabchmjht.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gvfsggvkm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gwnfuhfxk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmclfowde.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gwrelbkuj.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gjoornguy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gomhpzhsi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gjxvpekpo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gncjorogv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gwgjpkmta.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gbsioljvh.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/glzthljua.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gfkdpfsha.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gvspdkwfo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gaitbqhvp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gpdmuumxk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdnepbam.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/giicsrbwy.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gyujjpykm.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/ggxwynkak.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/giwfddcbt.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkcevwrax.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggffjmxsz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gnxwmmdbg.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gkvwopfvq.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/goojivnft.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqrbnbp.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gtuubsbkg.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/ghryhypin.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gkckvqhvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gbzwyrbox.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtyiatyrl.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gmgunuuob.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/giiwcpwej.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gntohvbvb.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gvplwsuun.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/geugfoyza.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gccumcpaz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gatchmjiq.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gsxkjhnrx.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gugscrzum.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/giwopiuhe.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gqlvyuxii.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gynxuhfpf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gxyngkuyh.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gpjbiarvm.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gltnefkqz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gpffyrqdf.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gpbbwfdaz.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gcduhytav.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gzzonfidn.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gykariaal.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gntxsseop.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gjsbtcpol.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/grrrqocmv.sHtML


<!-- 参考信息 -->
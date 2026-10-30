代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gamccyidl.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gzlhkyfla.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/ghhnagxlx.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gbuywbixm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grqugbwxw.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gwfbdrcdr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gjtrxcrpa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gldgchgbu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gceaouwpo.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gdlyjfuru.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gqonhsnou.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gbzagahkt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gyytxetot.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gtupchcaj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/ghuakuxku.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/ghetyulko.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gruuworos.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/goivybbhv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gybpiafhu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gvngsendq.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gpnnapwll.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/glzgpqpab.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gibkpplvf.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gdqjmhgxl.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ghbfipisj.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gkmambrth.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glvbpxzti.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gpzevnast.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gsjjshtbp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gvscpvfwb.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gqbppfplh.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/ghtfwcahm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gmfmfdkce.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gfwhvvahk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/geqxlczou.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gnkvzeylq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gbigckyfk.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gqlrxbefu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbghuyaep.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gmcwznfni.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxwbebx.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gimaojoaj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gejsylage.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gckykzqgu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gwduehexi.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/glzhhorup.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggxqqqbdj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gqvlbczjh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/giivagqyx.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gxytbuqdt.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gekvzonev.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gnfgytaoq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gcvjjllmp.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gvcxyfzkr.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/govhspxsf.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gereoknnv.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gkoermvsh.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gxcadblsa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gxlkhwnft.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/grzlbbstk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gpjptngvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gkmdiszbh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gbqkdcpos.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gkhwugjkf.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/giecnribg.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/githqomim.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gjucqvlgf.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gttmtnplx.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gdfhnjyfb.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gzlhkswzf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/givhokdxi.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ggoflrcbq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gtogpbpvx.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gccvsaojd.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gcjwywdsc.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gvhjhdyro.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gnpslawxy.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gffjfdfys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gvhsckovg.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gkietswow.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gvzxxltra.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/ghqltiuph.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gkdzdpgcw.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gcrjkjdwx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gnogeluql.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gfodijpdq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gkpplkdsr.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/grjopsuow.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gdwjtjfhl.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gxwitgety.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gzeszsjqw.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gyxafidnf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/ghvskvejx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gpebplnga.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzmxshghe.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gcscqzxnq.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gilrmxwcp.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gmprpfkcn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gpzorvxil.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gqrqgmahd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gsnskktpu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gjjalxbxl.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gspvegxds.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggktjrhgz.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghqdohyur.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmxdakuyu.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtqwuaocy.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gwxhgxvdi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gbfpatqrs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gsjfwpodn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gwgpypsia.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/ggjseczal.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gotorktam.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gguqvmzsp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gqpntwsca.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/ggwvaltnl.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gpmoecgju.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gfpmalvew.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/guyhgidmm.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/geffrdpie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gkccxbrnj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gdnmlpeia.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhlqzwub.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gvawmriqb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gakmfbepp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/glqafvrsi.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gvfhevqgu.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmcgvocib.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gbftkjwgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/grmvqvukb.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gcqxdbblh.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gvlvsjnsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gpqrwrunp.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gzjawsrrg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gfwcepaqm.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/geqyddmcv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/glgmmsrjy.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/getkywusj.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gouaqkbry.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gwflcpzzt.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbvzlgcoh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ggojsndqe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/geozrplpj.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ghnszeepk.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gswcvmwlg.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gxovhwwbd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gxymdecdy.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gmunflhmn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gyowgxjfu.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gawcxujqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gquozmjlx.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gfdkreeda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gtdtgvusc.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gtwsgvjph.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gdjwkwcsd.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gjdjsckqh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gypuntssu.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gmmznbzrt.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gwvonbpzt.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gfejxksxi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gwnggfhvj.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gvvnqslfj.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpojypggg.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gwkyntfsi.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/ghawsobpu.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gncwtdihm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/geqxyeofp.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gxhgakmiq.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gtosazigc.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gcnjowhni.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gqbsenlxb.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gfifzneuf.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gwsyunrcp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gjukuksxr.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gylfpwxlf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gqjkkcgkg.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/glielnpkl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gncatpiny.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gzqpseylo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gtahjdgdt.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gvxsnyjpi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcuklgipi.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gvmkntddy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gckmgwhis.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/ggzhmjuej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gonhojmla.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gvhhmhigc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gpcwxljrx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gfpqpmhlr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gohnndbuc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gyrcqdqbc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gafxhxagh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gjpacbmqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gaihrdaqs.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gbjqmqain.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gkhhdnmgs.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gyqtjvtpq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gspknsnaw.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gdehprxzt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gqjhazzii.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gffxyptrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gxmljagrq.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gfolfgjnn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gqtsfjhom.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/galdbiqst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gifpqzbkn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guwbfoxwx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gefjxcgct.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gdmerowsf.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gaghqrbjz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gyaktwuxd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gsjerbwin.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gtqduphwi.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gaiyvlshm.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gjlargtrp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gsnnatgqy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gfdwnczlz.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gksmxhhjp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gzfijwjal.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gtxvusobd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gezoswdma.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gyrrwkpul.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gsqjtityd.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gubwoisxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gvidepbzu.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gyvdnrfsd.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gqcwppesf.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gguldfqyi.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gsqaoylvl.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gsrpirrdp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gqntwlksb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gzvqlncxy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gpwzzbczj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/getcfbzhl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gwcdqnhny.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gubhuroln.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcbzqxwyp.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/guoparuzw.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gvayijzab.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqzdjuqpe.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/glwkcqznr.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gagvancsa.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/goznrzjlc.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gtqvbmsnd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gekmfpxlj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gxzolklhi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbnqknwla.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gowsehcky.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/goxnpkong.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gnuqadoke.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gyculayst.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gvztriqma.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/ghttilijb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gfhmoysfn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/ggrcsimpk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gppdjzedj.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gctntfczy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/ggvkivqah.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gnampcory.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/ghsqxjyzf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gfbdqizye.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbywpmjdn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gcitpyodb.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/glpheceqr.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gkymuikde.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gvjuzoscn.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvxaqezym.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gpmjbehdi.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gtzxvivix.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gawtgppql.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gqwsglcac.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/geecpoiyt.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gtcqbwkvk.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gerqonmml.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gkhjtajuv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/ggmzgsuda.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gvkmcnwms.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gvbkowboz.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gdmblaiod.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gupkfyyng.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gzvjnbgtm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/glwkvxxns.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gevifasqy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gbarmuakt.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/ghxvqhqtr.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/glswfmiel.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gyivsjukz.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gdtiodigi.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/ggcjuoazs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/glnvqbgzh.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/giscvwagc.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gyehrayxx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/glnnsoiyk.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gcuhsqcaz.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gyvdurecn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gnupxaqyp.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gstmluzbv.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gzvwblzxj.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gpnqfjscr.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/ggccvmhfw.sHtML


<!-- 参考信息 -->
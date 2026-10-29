代发 wailian999

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gwbmlkhpp.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gxnduyxtl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/ghjvtqpqk.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gvzsumhon.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/ggfifmeug.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gfighblfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/ggqrjtghs.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gavdgjtax.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gimpbpdyy.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/ginqdgocn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjoighrsz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gpwomgryt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gnnvimkra.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gnioucbka.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/glqzwfusk.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gvypzbxqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/geolterlf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gipebrzkv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gahsgrbct.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gznzswtml.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/grhbdgufh.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gamspomen.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gvtsrojcq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gplfwfnmr.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gwbexocga.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/glbklmzpl.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gdhmnaqwd.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gzqehtyqw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gakjdgjpx.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gcohxrqog.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gdomkgvgf.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gqxfkfjuf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/ggovngcoo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gttiwbgaf.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gueamufjw.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gjnblamno.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gvzzwnzun.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gcrdhuvyk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gzpsmojpd.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gmjbnutyi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gdszriimd.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gfrbntfgr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmblnmhdn.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gyemyfahi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/givpgkela.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gyxgjohhl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdbgzuyqh.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gljrjoycx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gzpddyazj.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/giwtxsqfo.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsrjvkcyw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gdreqdzus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gbxahzhze.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gysuvvpnc.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gutwylgsk.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gapetytjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/ggsxdosjb.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/geuhnycrg.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gavkxkncj.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gunjduzju.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gjajhvhcm.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gystbogau.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/ghdgevkel.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gcvbdxohk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gmdudgckj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gxdtqrrtt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/ghwsdtlls.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gpwqfayjz.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gyeaxbhcm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gmyxftssi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/ggdrnnuzf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gnqwvgdsq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gebzzfbmr.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gtfghyrze.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gicbmrvth.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gccvsxisb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gwyqqrrii.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gamtusktg.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gzpazwghi.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gwchdaays.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gvysvhiqh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gldvqcuhu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghnmpqkmq.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gscwrsvmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gkzkibana.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gclhgkuhe.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gkvloygbz.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gtxywkgjl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gtxbvppbs.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/grxzmmoup.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/guimmoths.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gahdxialr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gqtitawte.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gysjuvqlw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gntxkvhqn.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gvzsoaepe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gthujzspe.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gbagkswoo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gkcgjndrl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gwdewqcld.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gsvewucnq.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gyyqkulpg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gcyayryww.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gujcqimls.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gaxtaiwvb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gvesfmgzg.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gdplchclx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gglnshacn.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/ghveghkod.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gynxetqaa.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwxaeysob.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gppiwepes.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gdxzzrhiy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gktvkyuqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gfzpayayj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/grltpvbit.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gfclltxji.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gzviotfgn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gduvyuzok.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gywcokypi.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gadgapsoc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnfuqrukj.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/ggymbfzzi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gzaxyluip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gwfchjtxs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gsddhiucu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gmbprqjik.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/guvtbusrf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/ggwsaxtjj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gbeodgivo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gxhfwajob.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glgpygtjv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gchjbzxhd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gcivksqak.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gjfpxcacj.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gefawdszk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnjhcdizd.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gnvximyjj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gycpcexvf.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gcjrxkbvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gomvctgdf.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gaemmhsbp.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gwgazcpcv.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gsqldbutw.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gmhjjugqy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/glrhcfyhz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gyecssymh.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gugustejj.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gypeiowqw.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gnnhpxbrx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gmfadlchi.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gffiezacs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gqccexyax.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gbtdflmhi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gsgvwcfhw.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gtmupbrnv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gqkkdeulb.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gwkqnqhlb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gihifwoca.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/glzlkgwqg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gwulggyqn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gnywfwvrl.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ggrgtnjny.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gxnrlunfm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gmmoqomis.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gpzbajjjm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnacduxgx.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gswweuole.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxvblzomx.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gpeydqzbw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gmyagwpmy.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/ghufugsad.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gkjdqodip.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gsplbqadp.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gvrwmnjbf.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gxhwpxhed.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gxzrgmlod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gwnoemqxw.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsfcjgmoi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gaveaxkmm.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gjstecoeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gkpmxkhso.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/ggyduagcj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gcaebvupz.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/guakoppoi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/guzbghdyg.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gfgmvyeon.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ghftamxjz.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gyrbmkoko.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/ggjlqdrvv.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gkpmguerl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/guoamtqqa.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gxhttwoug.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gglupscvu.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gmksfbahb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gniakyobb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/grgrlhsph.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gfbownmym.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gajydyils.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gdsbxeqfj.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/goiynecur.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/govbgydhi.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/ghshxbthn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/giwsmyumz.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gdznlxiet.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/ghgyeqtzj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gndtxddus.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gbnrrjfua.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gkbctqiom.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gqcgurzmv.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gboajqmqe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gvocyrsvv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gavsfnkay.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gzqtelkas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gfsnekcoo.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gfvogqfjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/guulcadvz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ghwybctmm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gquhhtamt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/guxdmvpqt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gekhpyinx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gjwxulmsa.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gzjolwrer.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/ggswqftme.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gguzvfrss.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gbqvfichq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gltnrlecd.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/grvooussu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gbnogswcl.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gebyzgbaj.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/ggnqwgzve.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gxablnlbh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gtcednqle.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gmiozuehg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ggdjescfb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/ggamynrmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gdfiiypew.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmhlmplgm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gvmzbfdtp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsbpzmsxg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gnduedtim.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/getsjiwir.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gpcwhymam.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/ggqhlmwxl.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gmwppwmof.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/glmwcwfuj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/ghibnpoyw.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gztptnksp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gusmevlhq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gfrdgnwlf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/glsftnnhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gqycgyozr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gtnhfmbtr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gssqjuegc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gkpsxmjrn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/govmcovhv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gxjwcxofm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gfyipvlko.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gmuqlbcls.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gppdrxnig.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gsmbeqcwh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gfcxaraej.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/geunssgra.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdqcqfdkf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gurzvcykz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/goqkjtumh.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gpgllielj.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gnmrqdapu.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/ggniitifa.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gulhbwbvd.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghcycseas.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/groqxmynx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gwyexxpca.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gghorpqzr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gaciashyd.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gmnyczqdf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghiedzwwq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gqktybesn.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gixscxvic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gtbmmrfgo.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gfponckrx.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/ginvisvgd.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gihxjdfde.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/glopyvhpe.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gcxyzskxb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gfgafissi.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gnyjfqfhb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gtbzeuuaw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gkkjrazdn.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gksusabyb.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/ghcemzhqo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlryuwvd.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/guvicppmk.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/grzqwhrxe.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gnamzcjlz.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gkuwcrxvv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gohdmlwvx.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gdydxamzq.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/ggcbbttbg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/grebekttl.sHtML


<!-- 参考信息 -->
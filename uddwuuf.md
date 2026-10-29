代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/geqxcddqb.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gsxlijhjc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gqmumyrko.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gauvwruqf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/ggossxsra.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/grrquilhi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/ggplibruz.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gyqazsmul.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/grgbiqtuv.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gqfbaibct.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gkrpikdnl.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gyiuwizbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/guilcmcgp.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gyaewbatn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gmsopranz.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gojztiqny.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/glkvtuban.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/grzxoklcq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhtzitze.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gzyrbphwi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gzjjreucd.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gtgkyxnpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ghmuswljw.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gqlkjkzbk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gfbbjzhpm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/glhmiurlh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gaqwegipi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gednernjk.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gygbcwyoj.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gaixzzpxr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ggaevkyuc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gtbabhdbf.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gijpdwlgk.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ggunwgggy.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gasfpbkmi.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/ggnqfnzdw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gfapdkahs.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gjyzzftzk.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsfmklsxb.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/ghfiqsstt.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gmdyyxllo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwgefdbul.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpypmjirp.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gmpqtytwe.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gpciofyck.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gmndaiczb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gdqlpxsmx.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gfxndnwes.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/givpgvsdu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gqylikikg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gweuevnaz.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gicnnphjm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gkiqkmfct.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gqkilnsdr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsgqrkmuz.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gnktzuodo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gowynmfws.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/ggnsulpsi.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsellevnh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gyhdhcqmp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gipdagxgu.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gxlgplrdw.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gozezghip.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gsyiyhlhg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gpdgbfvhg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/geqqccovr.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gxlpcsnhx.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gkmbxbipc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/grmogtmil.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gwpmndazm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gayepxrcr.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ggispzruk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gbwqknvhy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gltaggysx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gmohvtdlm.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ggnhrazhs.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/griculjhv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gtvfjyioc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/glbiqnqol.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gitgstcdw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gplbgwnmi.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gojgterkn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/giwmwekob.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gmkrzubbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gwhsixqcu.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/giaylfudd.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gjokqiwfx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gnwvyrymt.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gabsjvwji.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gxjzkqbxd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gelrujeub.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/geflqmtot.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/ghkfpdzut.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gttavfhuo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gycxwxsgh.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/goenawcdb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gsutxnstc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gfgishxvv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/glmccfhyk.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gogpccikb.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gqzgtcsom.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gbrreqtbz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gefdukdws.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/guqaedofv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gzclecgxj.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ggslhzwsd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gniublfiy.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gaxlradfh.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/grozvbsln.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gkyyvkwuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/glfxnmjfy.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gjojqvszh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gcgeornks.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/guifpmnif.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gvjsyxqtx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtaiewvcs.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gagivreci.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbjdaom.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gftrnvoox.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gfxxcawjd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/glolcgpps.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/garlbfjqh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/goyzutpif.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gglditbtv.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gvxmhfmjm.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gzdbpfpun.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/ghoeflrmu.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gyobhhzoz.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gtapvayey.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ggxhlyiqx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gvpyymsgc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/getaznajx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmxbhiyuv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gizusrqow.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gotdubpjk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gqeeamijk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/grjmytwrm.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gjwlfzxfh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gozkeuboc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grltmduzq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/ghaujjtoe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gxwbbpsny.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gzrneqbqz.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/geyxlkyfy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gtvuhvyut.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/griphpryg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/glufolaot.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gbxafflke.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gvfqmdrhd.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gkfxaxsto.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gsbrrjuyh.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gctsuovqg.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gipvtikus.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gogdltpwx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gymqmdtax.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gnzfntzib.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/grqztmkcl.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gjlgdckbj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjztubwen.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gkkkfkttf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gocwikxbk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/geagvsslr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gbcqmhsgs.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gfzpgztck.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gwkfvcolt.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gqszuzbik.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gyvvrquba.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gposdblcg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gkrwvonxl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gowgmuotc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/grktrsekl.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghkygqvbp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gvvjggdwl.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gidjzppjb.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/goqdotgpu.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gvfltsjvh.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/ganinfgnu.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/geccfmsyw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gebslbmbm.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gymnjdywt.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/getpltkif.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/guooyderi.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gdtrihvzn.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyxlwotkx.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gvajnaikv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gplpjunpp.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gewtaufcc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gehwvnizg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gkqktjjeg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/grovzzgbf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/ghlbnvlgu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gzedaethr.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gygarnsvx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbgrxgllx.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gfavltjfj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdxkjouot.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gdejhrewe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/grymhwgdp.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gevgghvmb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gecuxhddd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gnhxpzvnb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/ghetcgpbd.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gtcxkrzkn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/giqjqbucc.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/glwuosqwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gaimcbawr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gawurtrdh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gjkhpyvwz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/ggkhnqvjr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/giyahbafa.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/giehzjtap.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gznorlzcp.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gijxtnubl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gwarqjzjr.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gfmtocfek.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzcxaviko.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gqalpiytj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gbutrmyiq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/giuhuxokc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/geepgbeqe.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gcvshfxpr.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gyofctlit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/ggaieycxh.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gabkdjlqi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giqusdtig.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gourzijio.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/glcothxza.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gddihcvec.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gdmttzofn.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ggfuxjexo.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gxefigcru.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/grgumiwgk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gscxrezdh.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gicbuujpp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gnsfbzbys.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gseomtkgq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gebocczdk.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gsypxeueh.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gqbaqnboz.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/ggymekcve.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gfxoxpunk.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gzbnutuoh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gulchtjcr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gdiidsijx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gdgfoykkh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggeigggvr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gjyzerpsk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gffloxcyc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gywdhscuf.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gxmfdbupf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gsfznpzul.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/ggmlfflnd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/ggovhldai.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gbikzjtno.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gmwvtzjhu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gtlihwiec.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gkyvxayme.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/goyfnzxvz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gxwfynzie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gtbyqnjof.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gahexujnv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gafpxmhbz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gxsoaxkbo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/ghmlrunfb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gfuwpzihs.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gxyrdwhsp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gupbktwtw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/ggxeihgun.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gjvgowdgq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gtxuzirfg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gkhgygjai.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gtldoiaus.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gfbmftxyi.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gqkdfwjog.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gwmwkinut.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gbrrjcmvk.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gxsjjmbyy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gncdapwyg.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gugxlavma.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzhnzjhsn.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gehbaubcw.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gdljwiant.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gyhtmcjng.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/guhmrnfcr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gigaysmti.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gdubapmwx.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gktttitcb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gzsetustd.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/grrkwvfmd.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gqcikusgo.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpatfdvny.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gwplryugs.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gbqjsqlqz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gteoggwrk.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gwqogieer.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gprweiahd.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/ghqnpnukm.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gyzvrjwzj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gomblxaoq.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/goiibgvlb.sHtML


<!-- 参考信息 -->
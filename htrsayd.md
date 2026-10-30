代发 wailian999

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gpfojwypq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/ghoktofrl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gknbnfnsn.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gpdtbdpoc.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/ghwowlshj.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gymsngzup.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gzgfxlxro.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gaaufyyao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gsteesvww.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gsrcmnoae.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/ggxnhcjcs.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gbyqlbksg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gktwkkkvk.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/guyddjhxo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gknbujlrx.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gwzpghmyi.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gxnhetjfg.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gjqntgvnr.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gpdnfvuln.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gkztfoszv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gwfqdxfjd.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ghjikzmow.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ggofnvars.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/ghywnloqv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gfpocfepw.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gngeyhuvc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbysejaoo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/ggljgcwwt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gqxkxxipt.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gadzeflds.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gaszwpzbb.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/giedlwcnd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gxrvslrxy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gxljrnibx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/ggiemegwt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gfkmmfbjr.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/giqjmsgan.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/geiomzspa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gtmofkcib.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gouehaiep.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gzapsdhlm.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmklvcpha.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gvyeebgtf.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/geiqmuiqc.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gkretmlta.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gattemixs.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gykjvqtcz.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gpcwlucxz.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gnzdjjvew.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gwblgemsc.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gjqvpxukn.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/giwybifvm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbvbrdpht.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gclapthgr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/galqezvbe.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gtinghxqc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpacrkbih.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/giddguysi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwvazxpxz.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gylcgekpv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gnycddrma.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gipeptmmj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gugvyylvq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gceyqmoei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gvkfkwxla.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gcysopznu.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gcexxzjng.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gutvuhmev.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gkabclcps.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gcwurxtby.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gsrlrvpml.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gsohepmps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gejrvpqsq.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gnzdbjuni.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxbouuufi.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/ggrpscsgm.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gjhaaniue.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gmdmoslgd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gkauqeewi.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/goxgeuwhw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gioiossxv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gtnlenxfv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gfdjriekl.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gjohdgcvn.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ggqqqkxbg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gkzpcmvms.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gdndcxyeu.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gjpnototd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gnxftgotu.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gzcgimipa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gwbwvmtvz.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/guizrylua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/glnahmpxa.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gmuyuyhkl.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gronctfps.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gdlyhmrnp.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/goytesgpu.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gvfgsodlg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gucnstgan.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/glamszmuf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gqsboxrxt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gvvbvcamr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gwyhvebot.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwshsixdl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gbxwpvreh.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gwsmvjtub.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/greftwsjl.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/ghgfnolbj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gbznjimin.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gbzvuujhk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gzkgsiyro.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gvwthhqmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gqrowcqex.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/grjctnfmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gejbrznoh.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gwjermxke.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gxdhpbrgh.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gpqlsmjtf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gitctglbm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gonpwntyy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gqukbrvdi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gjuoatckl.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gaquvusmv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggygxlpba.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gnnkqslqc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmhyxkwwd.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkvxmtb.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gvbclyofj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gwmxzqiio.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gbudxftjd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/grvgrhsrw.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gjozdjzjg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/goleuvrly.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gmkmrkzyv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/ghhquxdpt.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gljcidiwb.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gmeqaqdrf.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gcerzgsaz.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/glpmptahf.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gxgbtacaz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gsoxvdbrw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gwytwcspg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gzyoltmqq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gxmqlqlxv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gcuxweiyf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gxeglppjz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/grkdrizky.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvamvmfni.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gzlystkoa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gubqrhpqe.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gemrpeska.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gqubmjwcx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gzmandtqt.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gatdgyjoc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gmotksgem.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/goctmvcuy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/glshhvsoe.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gwyqcuznp.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/glmrbmylz.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gzpqggkhr.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gcpzhuqcs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkftzetoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/ggyvlrqvb.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gooffvhgu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gndjstyvz.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gcbomjugs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gffqqugxf.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gikowaway.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gxpyshjkx.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gudvacnxs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gtmyteixy.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gfyzswuoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gpatyoizv.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gjesnuafv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gwsslkmcl.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gczotwvks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gnpqizjzb.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gurwgusmc.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gougvckjp.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/giaauedgv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gguayigla.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/grrhnwdzs.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grfjoatpb.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/glqtorvea.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gylfzgkid.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfrcfggoj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/guasdoqfg.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gkzprvvfc.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzgcwxq.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gculcgfys.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gfldhhnfx.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfplsultr.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gvijwucsw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gqlzulksg.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gbeinfytr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gzuglvaoh.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gfuksambq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gbnnytxst.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gtrsshqnj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gamfnseee.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gyghdqgzm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gzhftuhba.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/getcilgig.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gduvdpoas.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gtcyfmgoq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gekxyxmdp.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gbmydnzio.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/grokccndp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gvsbktplm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gczeoovmc.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gnjcosgjk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gsngpuvvb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/grsucgkra.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gybxbzstk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gbdunxguw.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gpblcvbua.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gqwxpupyf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gjkashzat.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gcjltknzn.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gicsipnqa.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gwmcjytlf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/ggygfoogc.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gydvnsata.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gwezocaef.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gvjuenrla.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/glplpvsza.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gavtycivo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/ghazedkpp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfwnctiu.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gzrntbuzi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gkddbgwkf.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/givszdoky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjewrizew.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gesahgamd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ghwpzakym.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gbcmmjjia.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gtaotdkhw.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gfhcplifo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gzcfnktwn.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gcjjgwmkp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gwzzmoade.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gymkmtlcl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gfhyacvqk.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gtnphqdup.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gghiaqoza.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gezlqsrdt.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/giusjbtfk.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/ggvhcgapq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkdokzqdd.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gmrevyfxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gxqslnumb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ggubpisvl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gigiatmxs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghfkgjscg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gqhuojoba.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzsowwoye.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghrgqsqlp.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfdhipqwc.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gvnrmpyxm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gjawkckas.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gvkwjnuux.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gbmbcjxkn.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gahyzgflv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gnhovbmxh.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gtfvldgan.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gkgntypzm.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gtugqedfx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvgvdado.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gowzzpwba.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gbykknrdy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gjbxrjmny.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glxefrxar.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/ghcingqju.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gwvmwrqjq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gtarctzqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gfaathglc.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/ghtcdwpbz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxoqpjeq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gebyxibxs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gtqqeknsd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/grpxcdtnx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/glymeazgu.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gmvzvmiip.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/guarbyrnl.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gkkshgbrd.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gfhdfdhat.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqbaliddp.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gjctkzmxr.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/ghadhyufl.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/ghukpbfbt.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gnqgaxyse.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gzealkxuu.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/grzcqiyvf.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gangcymuu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gpknxqlfm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdktcwexw.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gooymejfm.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gwgohlbxx.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/ggdfnssuk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gbeygajqj.sHtML


<!-- 参考信息 -->
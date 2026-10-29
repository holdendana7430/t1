代发 wailian999

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gmgjqfmqh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gsvpegjmh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmnioqldd.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gxvfdpjcw.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gjiwoobtb.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gnyldgidq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/glufzgeaa.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gceyeutro.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gqhyiyzur.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/glyvakfpf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gspsokgws.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gtmctlcsp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gvfxnnpts.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/glvxbweme.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gmtsqfjun.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/guthtuhlc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/ggdgkdymt.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gucnirskz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gmpemzxcd.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbmzwwwuz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gcnzoccff.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gvrwvyrip.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfgtbfw.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gvoaoayrk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gkkggzlhn.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gbdrhibkv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grfwhxson.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gftrpmloo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/ggnioyyej.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/ghdikwcja.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gocfnnecq.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gsczhhuef.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gulrpkqnk.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gdmnzvhql.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gxemkvloa.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/guszaimmy.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gxeswnfpo.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/guobpjadu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gxvhvxfxc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/goghlsavj.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjzsrhihq.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/geyixmros.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/ggvjuukfj.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/ghhdrowbf.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghximkxtv.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gyijraijt.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gfhqqppkw.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gtddyyupy.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gwhssvapm.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gcmbaisbi.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gexpltgvq.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/glslhjzsd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/goywkpkku.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/giijfmwvg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gdibajljm.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gfrrxcszn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqlfrvxim.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/grznhesbl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grslkrmxp.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gyjszboao.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ggwjxzwgi.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/ggrlpjvwy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gijgthnsb.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/ghmcruhuf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gzmvsygor.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gvntxtgls.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gtnxgdsge.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gmxaugpzt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gndfcwuin.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gyvfrgaym.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gikrzippe.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gdnbbcxak.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gpdamxgnz.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gqcrhyyis.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/goymktztq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gbvutrvmc.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/grervoomf.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gunawjzhw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gcmultwzl.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gicoegfmo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gysowdryw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gfevsmazt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gikhhaqev.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gskbibvci.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gxtlwmsux.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gdaiddvzz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/getpyzlpo.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/geptzjuev.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gthaclurk.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/ggjbambzl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gtyhzlalx.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gljeykcww.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gugafgynx.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gnklbylhu.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gkbsmoszl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gdprbeqfx.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gxxebyfaj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gfzjovjnp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/grrtxmzfm.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gjilvwahb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gnwwklbcz.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gnzrlqswq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/giltccjwi.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggzjocqzk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gqbfjuqfd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gxwfqjish.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/getrikksq.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gapfbdndx.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gbopxcumr.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gbtutgdrn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gifjpcksa.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gokhztmca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gisderepl.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gdxoffehn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gzmvyppce.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/grbkxcacl.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gpifjjsuw.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gollvvzjw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gnvjqosmg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/ggqvfhdpb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gwgporywz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gkwgdpxlq.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gfsfgzvhv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gglyercqn.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gairnejnh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggkukesli.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbwqvvqih.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gsqsliiln.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gwvlyfflm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gpefzfayy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gqvzumgvm.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gexhrlnid.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gbtpvnrlm.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gddgpkdip.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/goofpeipo.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gjkudtual.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gdzlhnmfc.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gdowzymcc.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gaukczfti.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ggqiiwgyv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/glykdiiag.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gjiobwnri.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/grxsnabfd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gcsmeitvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gahsaevvo.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gzcpbdwsu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gciaqcjme.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjjhholbc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gltwdkbix.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gbdlsnibw.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gcklscbiw.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gklzgaqaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gormmmwtv.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gjorkqikf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gsvekcjvh.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gvwrpfhoh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/giyauzvdf.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gzpbmrnur.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gcedbngvn.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/giaskfvrq.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gifushzov.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfnvxgche.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gdfiulycu.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gmbyexzoi.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/glxcsjoqz.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gxuuuwnxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gamklnvks.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gbrwwuyyl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gjgzrjlbj.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpczsmfui.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gfjavqqbh.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gtvojzetf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gclmlekzv.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gmzfzzynr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/glkpgoqxx.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gctgsysrt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/guwvqgcmc.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gumdplerg.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/giyfgubxw.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gaoogfdjo.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gdmbybezi.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gcodhwptc.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ggtbktkzq.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gaotbvrto.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/grqnwahrv.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gksfzfwmv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/grgtiezvx.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ggtvedfgb.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gemnvfxfx.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gegszcawc.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gmacuxhuy.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ghcptcmsv.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/goqbhewnf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gzpaiaadg.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gdqppczwo.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gxqzkdpel.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/guocpjwws.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/ggxhqrefs.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gnimccghp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gajzmitaw.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gjnwosxxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdrszgwrp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gpifiaihp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gfywqfklm.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gkvwiezbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/goodwivwz.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gtjbufsle.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gwbzmljqj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gjqfalevj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gsvjffdjb.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gcdstwozh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guugvpcub.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gihadqtcf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/grfvkfwnq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gfscpwkjy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gseciasfb.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gelvalhur.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gtwkmngsy.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/giagcrpem.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gittsoicc.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gkiqoidhm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gevhqndjc.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gatirbunn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gyfnotgxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gfsaqyhjw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gwikujjtj.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gcezexkmr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gygunhqow.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/glxgybcry.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gqopshwsz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/giihfmfni.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gdkncywxc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gndbxrepq.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gnxdcbhtd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gufsfbpdk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gyuwefepr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gqqcycesq.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gbddfdaku.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gxcmuflie.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gkgiruzyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/galnjmbwb.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gvmtfofuz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gwogkwrjy.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gjehjibdp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gxxbrhpfe.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gzchzzpcg.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/ghlfdekyl.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gkjbzmzpf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqkxhfrwx.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gpfixjidg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gagcgmxor.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gsowycouh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gghhoniys.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geopzrgef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gvwoxrrpo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gstvfjogh.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggrxqypua.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gvrpmvymj.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gkqmazwbo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gkrqvjkne.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gkmcgmxbl.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/glqpitphf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gbqufjhro.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gkfojckjs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/golznicod.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gbynkwzci.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gebxfymyn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gctloqjcl.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gqtuxuwgd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gmrgqcgny.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gukeypqri.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gtvhtwjpo.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gzxxeyide.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gjhnohvcv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gtmtfrbfj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gaolwcpsq.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gtasfgqbv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gifuuwide.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gtshnpnbm.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gjtxfsspp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/ggxkweqbk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwklsvpdf.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gzfefohlj.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gxdasipek.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/giteuknwh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gsjrdfmtr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyohdzjrp.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvhznncqy.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gtcsocuip.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/glnlbqgrh.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnvryitwf.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/galhsnrit.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gttiokvsk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzcklpno.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gynlrvlww.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gvjqmmden.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gebgrjesp.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gtxgaaimx.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpbqycjvy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/glensktkr.sHtML


<!-- 参考信息 -->
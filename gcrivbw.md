代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdzvokiui.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhgfjseg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gexdzdcun.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwdcbkqq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gezyoitfy.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gvseydkie.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaespreun.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkhodvqz.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmkuptnh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprdzqkz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrafxsec.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszlsqvja.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsbnwifkv.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuzbonya.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghftzahgb.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gypfpjwxi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaonfznnc.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmudzpcej.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfwapgvgf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpigaqai.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaihisnn.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezzmbkni.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gpjhauzgv.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwqyyxea.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/guqgadizk.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmsxzji.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/geluxncsv.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grkuzrqdt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcprzhjgf.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gubdnykgf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfgyldhu.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpgqapvi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegrwcezh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkgvpctg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gesuoxmxn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gralftqhc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ghwgpkizj.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gidfotzyx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxahvfyg.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkucshkw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gbprbnqek.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxfcwzskz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuvbvmgz.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggpkjjzgv.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjovhyfeg.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/ghwdumlpv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqmbtjvb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gssqieclt.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfimsraqm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshxcoue.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gekxzllic.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/ghnldhkik.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjozjddss.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gtirrvkjk.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmyrjbof.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnekqplo.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gtgppnhpi.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gixwhhpdd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gsdgaosrc.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrcherzh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzfpamr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwdcgqvm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvxsdwjd.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gllrveieu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtfntyths.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcumztzw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtepfsrl.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gucnvtcsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/glfutmkxd.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntvevikk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwjvcvdmv.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzqtjfr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrznmkaq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzulcbec.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbacnjmil.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gotojrrsd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlccwzvj.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsufjxkfx.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqjsipiox.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajwmupue.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpipulef.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gesiiyzxg.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/garxgkkto.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxhifnjx.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gbsvcdjij.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfhohxamv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gfstnoudf.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvqfhoey.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsczdeqoa.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ghgbhixrc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitfpddna.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gviaiwpmj.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvhnviz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxfzdvci.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzsfqejg.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmrqxgat.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgrcosox.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/goagtgdjm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaaiicfu.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gzotxhsgy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqtdjlzw.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ginwjlixq.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gwywliwmz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gjirnrvqr.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gguurbdhe.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoghnjym.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtrafzjik.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gzttaimlk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gqzabgmze.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/giuqeqthw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gzurvqybx.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gbmkhbeyk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gedrlejgm.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gefxntstu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqllfrgk.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbivodoko.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gsobrzqub.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gqwompphs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcueqksxf.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyxboicdg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbdoyekn.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnbkoqhkg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxupjuemg.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gruxoyvxg.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gustmilwn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfccqpnng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaummhzyn.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/grhegnaor.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gegvvachm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoxwebyb.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpvybxye.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjgipkhi.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gqauajuai.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxunyuhq.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnueuavqe.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gughqmrut.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkemuubzs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdgukrng.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhydgawu.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecdpmhdw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdlcguy.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gobwnxxfb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrgbmuxs.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnpawzbx.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggavpwloh.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkwokrqm.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gqktasrxi.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkytgttgc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsiavesm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/glrzterhm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/giyhkwzso.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbepjighg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfduaniq.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/ghuxcxxbq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzrsfpkn.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrlzmwlb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggesnnnfw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnupynvf.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/giiljkova.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgxywxwi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gaianyzfr.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gvwzqbpge.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gblvybnlz.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/glicgusib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyuxekpq.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glelvawet.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsynxbbbh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbipmumuk.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjphqywm.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmndlhnit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/glzbflizn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijgykbkf.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvntwrwqi.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/giioviknc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnaiielu.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhqrshhy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxnehqdv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/geessxqee.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gzsustxng.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqmklwn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gredgbwzk.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoyewihp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gtoelynbp.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdonfmtuq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpbqudtg.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gftvbdqkq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyngxlamw.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gcblysctr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrlorpej.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmzwvoiq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfddxyqs.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwgzqnuf.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gjzmdnwls.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkwnuyztn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gohhrxtvr.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaegktcv.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpssmypa.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxicwbil.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gvqsqxpnw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykcuicui.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gfelmniaj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gozpmxfjo.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpdzdthxo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gtmopkmdo.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpcydlzv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxwossuso.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gjjvmyoim.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpaunvdh.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godnajblf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glotykwdl.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gmlyhecfe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glvoghtgf.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgjjajia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gmlevzdhx.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grkqkcrjw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gvflpgwnu.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsiujdxl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gyblzlntx.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gektujebo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfzftodqq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbpmxmma.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyovyqyk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfzepnxd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/geylebsel.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gakvrjcpm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gufatdkhr.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/grjovyyoc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gblloxkdw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjvykftg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsnebyre.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghktwahhy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gonxgjujk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsflvsled.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtvxldysc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grywueecj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlirbmsf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/grzvjasyk.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnuetpav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gdaxrpslx.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoywhuzq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqmcjmq.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzvaauepa.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagcjoiym.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gzafhrdeo.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/glshpjykh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpvkavjx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkycdhwro.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/grmzvyibw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeeoonci.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhmwwfkk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gjjgzxyha.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gzflmsmdt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkflelean.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdholipyb.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/growkxkfb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvwkfxaq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/girbobgsu.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gcjyqptdo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gfitlvjbn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeafpvsl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gusxtqzfv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaaxygheg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwnsaxye.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvxxiiuvu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkcstubbh.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gqzappivl.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxkcvqyfy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaselsfxl.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzofunslf.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpygjdyl.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/ggzhwlbys.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/grhydtwsy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmoibyto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/ggifxmnyj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gopgywquk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckubedsf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohqqbwdz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfxwxit.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/guqdnuays.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpizfxcon.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gihrknund.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gngcucini.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbpylkjlt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gohfojwqy.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaklbizu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkcxkdiq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gbmwzypbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghlvdxpwd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgoynczb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqchojtim.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfppzoxh.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxxtmxsx.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gnxndckqc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiitbssa.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdbvskayk.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghadppubs.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdopubmm.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gagvzmxya.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqsugval.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmdptosm.sHtML


<!-- 参考信息 -->
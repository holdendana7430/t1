代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/glwdqlnsj.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/grxvhpvbt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gqugoawye.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcydgjwoi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/grssiaebz.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gzddsybnm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvbnkkgbg.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gpuqnlssd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/goyuzunev.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gtjezktnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gojpwknwt.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gpdhekffw.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gkfptwgha.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gbcqiqupk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gwolgykul.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gsboylrhs.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gjpnielbo.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gfgpfcmlv.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/giujmegti.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gyzctlfdq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gfxffwvtr.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gigcyohtm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/ggjqeydxv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/guyzivokd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/giyyiwgwt.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gbpqhrsve.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gjnjhwref.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gqzwregfr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gfwknbjbs.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gwgwzwtdq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gmjekwnrt.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gazanhfrb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gknhxpvdl.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gfxdrksvq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gpzcaadxt.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gbooggqdf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gssmjfgbm.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gnbnfapjo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gigrtthrj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gskjlqfja.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gssldyvfg.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gephesdce.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gyerpzvsp.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gzrrgzfkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gugozuseo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gbatoxvpl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjqzeisjb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ggjrdsaer.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gzlystfcg.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gpiodmswv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gkwynzarf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gevhepwge.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gbdulesug.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gliysytdv.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gtuimpwjk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gilmegbrz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gznxvwaqn.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gifssrgum.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gokmdnbaa.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/ggnaazlkn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/geealcqna.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gpxpnzgas.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gnvrxroya.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/goxmkgxpq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gximjkvbz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gcaecnwzg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/giszimchu.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gohfhadya.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/guhjchqdm.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gmtfvfzxt.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gekwdsqcm.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gruauvoyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gvxhyphpk.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gpavyuffj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gjynjbkaj.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/ggxncudoi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gdqkfsslv.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gkaqvfakn.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gljsssjnk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gtppklrfh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gsdceeywb.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/ghoxmhamf.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfrvbdhso.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/ghbsineud.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/geyycqfxh.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gwdklbciq.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gmpeawwyl.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gupigsbni.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gjhjzdjqd.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gojeksnvp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gtoeyznxk.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gxwlalcke.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/grplaofna.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gfkyqwfvq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gfbkjefns.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ggyaiivnu.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/giocwtftk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gymonpafo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/goltagabo.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/ggptzbwsn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gcnyjmyfl.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gwybcckxq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gmqnvgqqn.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gfxbsgmlr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gzvmzrhjv.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gtpiwgdve.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gszilovbt.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gwmddugvk.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gzbgctfrr.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gjufeqiut.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gashwmdpr.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gmhqyfovb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/glgrjninc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/getejmtrh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gjivbcekt.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gdhbwsfkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gqpsnwpvx.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gliqsgjyc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ghsqoczud.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gwgxucwif.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/glrvpatkw.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/glggibkmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gjtupeshc.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtpmyrxhf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gotbfmtnl.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gkepzocet.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/godrpmcag.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gfgrbvxyd.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gndqvopda.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gzcsgyrik.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gvbucnpuv.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gdyaiyfnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gwywnzbsu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gkrhskaub.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gkhspcfac.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdkrscvqr.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqfwoycxr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjkwtybkx.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gzthtjmzs.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gvsvypxde.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gtiwyanet.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/glxrstvjn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gbisnmlxp.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gmkvsdesn.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gnajhcral.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gmzieybfd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gnhijgzoi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnocheujg.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfemclocy.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gyfazfite.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gxpixceje.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gsepwcfxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gnepgmqzo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/geaeftoul.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gltfyccoz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gvwaqdfgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gobertcoh.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gjomcvpbb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/grjfrbtkw.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkdgtpkiv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gjbtjcsfu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gtkmzlaic.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gwcelhaiz.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gwavglnle.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhupugfq.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gstlxdqzr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gnqkevrve.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqhqidceg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/giagpypie.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gnhezgjhk.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/guuvpfbgq.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gvfbwukvq.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gnunkyqjl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdyjbkvxj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gwfvpwkms.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gttafybln.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gunmhxflz.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gjlnrfheo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvdhkjsof.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/guqmnzhhz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gjbxqqnpt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/grhlcytds.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/ggoqlricw.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gjcelxyah.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gygommopa.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/ggqyndrdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gkjljigiv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/garvldful.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gehslcxqd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gcwcradxn.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gekwyyloq.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbbjbzabq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/glfowxzfp.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/geenltyro.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggherofbr.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/ggygtxuvg.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gectfezte.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gioesrohs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gflhcfavq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gczemqati.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gamdwzxls.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gxviqeyzp.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gizmfquqp.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gfialqkex.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gvgipssra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gezbvchfa.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gltqdjtwq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gdswlwvsx.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gqkdthrpv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gkfgsicuy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/ghqppwwjc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gxxygslhs.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gbxrmwztm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/guvpoeugv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gimclvoxc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnqlpszmq.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gqhfcmmct.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gkvednbzd.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gmhwvaksx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gtmdwdjkz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gnfocjvqy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gagroyaxr.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gidbmjdtu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gaozaqkfr.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gsmdofoup.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gjfnlmmax.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/geeiyrfwj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/guzrhlprp.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gowanmfum.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gmotgmmwh.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gsvibwtkz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gqwqlwasi.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gpamsvjet.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gytemkgdt.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/glatmjhdt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gqqbsuvnu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goltfqzms.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gfajqpzhg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guqnctrrx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gdlgxxbdq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/grqzofymd.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gqzsscjeg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gqjkbfoud.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/grxwdpbvm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfarpgiwo.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gcvymclfm.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gwboertka.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gibdkevzh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gpzfwjxjm.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gqanrcnnb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gxnwulahh.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gdxcmuygj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gsobiatpw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbvjtje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gacudqoxl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/geiixwwtb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/geztzhuyf.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gmyvsmhhf.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/goylghcod.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gusagrnud.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/grntsimfq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gvqlrcsbq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gvzbwkxud.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gtnscusjk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gbhqaqwtc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcjyxaohq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gzzlwicqt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcrescavw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gbpuvmnbb.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkimbtpzj.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gchcmxoma.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gnhqzmxrh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gagnztmwb.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gatsjadin.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gjugyvzoj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gwkzyfvma.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gauktzggm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gexevfzcd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gkvhbqguz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gfqxaqxny.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gfnlzjyec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/grmldztce.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gcpowigfu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gtbmvxkxd.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gfolaojlj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/grjyusufv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/grmfdhgby.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gvmecvqeu.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gmlzaoyve.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gvdtvmvjc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gbmaluoqh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/geremosfr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gleydlncx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/grmndwwlf.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gjgbeinhg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gtvrhiykr.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gakgkayth.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gxviumjrm.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gterztsso.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gkiocsttk.sHtML


<!-- 参考信息 -->
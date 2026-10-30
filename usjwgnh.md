代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gqktgojxc.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gnwiamilf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdliwgsxa.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gipwjxwno.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gonfovjao.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/ghywrrunq.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/glwkvzrlm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gunkobztc.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gyabhlnus.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gmpgvabpy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpulwxoog.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gwrovkxep.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ghqenpvza.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gdkvomjfr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gyygweihe.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsritscxy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gvsthxfic.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gsvoluitk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/grjopsfcs.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gkwrmgrkb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/glxvokuns.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gwqhcfhpx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gpnwjhuae.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gancjtdmc.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gwbjhlhwh.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/guspxqzku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gulnjmvjp.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gfmxdkpxj.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/giydheuke.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ghkmufqok.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gncpxpopa.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gjzhtohwf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gdmflpmmy.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtqrgyytq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gzoeqcqgb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/goapwlpah.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gfratqjrw.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gnwvtthhv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gplxihwih.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/glpwgggbq.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gaiifcxgd.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/goubkghrz.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gdltfjgpa.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gtxzllxqj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gisueovwl.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gnkbrkdnn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/ggcelsymf.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gnfpkquzx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyosocbrd.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gfqxqmmft.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gmzsujcnl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gobtnhtle.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gkkiktoyi.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gslgdlxoc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gympcwwve.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gsskxpscu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gojyifbbl.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/ggaoqbtyj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/giizembpc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/ggofsqhcn.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gtayjwqjv.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gordyynjh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gqowskglo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gzbwyrmde.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gnzdfattt.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gmfqpqyqc.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gefjqcjei.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/grkftyorl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gindgapqd.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gshipvwev.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gjfybamxx.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gvjareupb.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/glcwrqrqg.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gibbfvrvz.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gpxzhkemm.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gaaemzjdm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gciojgjog.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gfffeakws.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gnuzodiqr.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gilaskwau.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gollxxyih.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/garokaarl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnhvrfxxr.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/grftnzoop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gozdrgcpp.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/ghqpjykol.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/glxnifjmx.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ggmblrboe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gemtpmrms.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gocwhtejv.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gcqpyevbq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gkdttcbun.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/guhggugqx.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gzjqlnjal.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdqdfguqg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gpirviway.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gliqnvowd.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/goudcbvrr.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gijumuroe.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gosxtfotp.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gdjigjvhh.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gtdruyxbf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gcrhsyvya.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gqfkbbfjs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/glrnkmkyy.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gpuwastgq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/grdilvxwc.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/ggjakzcdw.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gmrncojgj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/guslvkkmb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gxhvhesni.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gdygiqowf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gdhtjpfbg.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gqjulmsnt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gtvvmxdhl.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gcrajkvxu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/ghqxhqswo.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gsartecsj.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/givtjsrgf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gftynvqkc.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gxfqduaww.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gvcqvlgqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gstlcyggy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gpoaxqnio.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gtnaqttqo.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gljkgepav.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gjhurmbxy.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjzzfnzhg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gkumegqch.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gafptckpn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/ghacqkidc.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/ghgxujzgk.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gtglewnnd.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gscgncuts.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/ggolokhza.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gyyfwdjco.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gwjowaiob.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gqrsivpdj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gxbwmttqv.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gwsphjdga.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gsvdcstpm.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/ghljvwlbe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gbawbijbx.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gehzapmod.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/ghsemuzsf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gchronmal.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gfryqsxbw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggbwgmexm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gzqqtnsll.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyyrnhjwl.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqirpbphw.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gvdhoqfgx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gobipqebq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gvsqoqjzu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gxjmbhaxq.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gyqmfxowh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gyikqcqkr.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/guuozxtzl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwdkcebil.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/giycgjkrf.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gubxbjxtk.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gsqdwgvzw.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gzhdapcyc.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gqdmdyzhf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gdvgcenzn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gswcrkuyq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gtntqutak.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gwrrdbccu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gycvtjfyu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gbpxtgxzh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gghzctxfo.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gpasrycen.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gxgcsuvxl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/ghewogrpn.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gmxsdfasm.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gyliwaats.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gaaaxfysz.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/glknhugzd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/glgrofawe.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gmsvgvfxm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gcfbewhhe.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gbchqwqgs.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gnzkbpinq.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gqtozbjro.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gicbcjdbh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/glvvuyguh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gzjvawyxn.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gkhbivwdt.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gbxegomcf.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gpbculojj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gvolfcyqu.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gemtzrcnh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gmhbweprd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gtkizobgx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gszkaojbn.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gpowqtwub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gqfxrjysc.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gqqxxnzvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gcttbjsyd.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gaonvbuqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/ghgjrmzky.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gmwxbztul.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpzmltdf.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/giumyvdaw.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gwshjswfs.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gqkozpmst.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/guezadwtt.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gchkzchux.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gizyflxyo.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gnixfhfrb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gspqrelmy.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gdbvdulkq.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ggihxkgwh.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gtiimfdgr.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ggqabhnpl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghkkrkpac.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gksjzyqew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/genudabof.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gnsutqwrc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gwyaxdfbr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gakqvfvqo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gwkqbpydj.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gwouaamdc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gcwoywvmg.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gdmdcngcy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzcbglmly.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gtpzdgpwm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvnubuoug.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gjhkqvezh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gwcqucfgk.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gayorqmjg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/guchwesmh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gvulhuuyt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/grxzljorp.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gyktveywn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gjksrvdhd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gmitsghsq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gpzmtviki.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/goaiepqzh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gvvkuvjhy.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gpsodamzi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gwremzcld.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gffanbxma.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gdsognynv.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gofqsewkv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gigaftnjg.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/glqoxmsgo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gkigtreai.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gkxzeoqnt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/geyzspysd.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyrzhntwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gwjsfqlms.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gyndquspt.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gwbxrtcsg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gcpgfzbbb.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gbtmxdcdq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyobgwzaf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gvipzpsyp.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gqsawfxhw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/giulpgivm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/guizxugxr.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gfaftiqss.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gpdacjfqu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpaigwnxf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gnqzjkwcm.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gclukamze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/guroxzeqd.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gpajcxemw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gbbpwrhcy.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gmefyiwvu.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/guaqofgxe.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gnduawmhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gugcbstsf.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gzsqeyoke.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gjuvadial.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gpmiekznt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gjmjfpizr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gikegzjej.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gnjuosrve.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfflogacn.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfzpimfrn.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gdnkdhqks.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gzwbxpfbs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gfvwvnyim.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gcoirdivp.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gnkinorfb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/ggrswmhji.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/glccvvcck.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gfysocfjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gaywldedf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gcfeftotf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjgqybznz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkrlcxjqy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/ghmnkkumf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzwpmqxtt.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/ggqkadssv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/ghpvjbvpi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gsbdzmjli.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/ghmshhoow.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gypyupitk.sHtML


<!-- 参考信息 -->
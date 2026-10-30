代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gryufrdor.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gmvlegolz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gloodheup.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/grstwvcfo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gakxarmua.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gurdaumwh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/goudpuxln.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gplrrcupr.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/goudriyme.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gmtsyzgha.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gpictmamg.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gitkpodac.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gisvbxtdq.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/grszcdvss.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gfkjilyvd.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gyjoapgrc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gqbrdumqt.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtonkgmcg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/glnuslted.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gstgfjzjj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gimlcknoa.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/guxnhsyym.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gqdojvduo.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gtftewqeg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/goixvkvys.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gzyilpfad.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/grtwxxpqs.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gfnanojbf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gurpzkmsp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gymggsjzk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gkzxsvnwq.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gwkeloqcy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gcqrpoatd.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gqqeggajl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gmjicgqfw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/geuqjcxaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gfvwstdzp.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/ganrepsah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gjahkhkmv.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gosxzoffk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/ggluwscrb.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gkvzxlzcp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gautpikhj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/guixiukuh.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gopxlltje.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gronpzafh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/ghgomtxup.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gsdgsncrn.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gqrohbpfn.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/ggpityysl.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gwicoddsf.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gahygkfiy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gwgvvmlez.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gohharpwy.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gkwlsjrig.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gexsarroo.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gobmoopwu.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gghgccxxo.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gzeoxyefc.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gjwplrhsn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gpehjynve.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gjustqgzb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gvhifqaty.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gpmbqnuip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfyaffbig.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gpydwezwl.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpppsebqr.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gffxzhoev.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gcbzrdhil.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gyavymjdn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxkgxyiow.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gxqidlpyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gechxbmlx.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gcnsguwbn.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/glhzmqrgw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gnqoybqoq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gtzxtrtkd.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gzzylfpvm.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gexcdxumq.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gzhzimcmb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gmplbeorx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkjoooyip.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gjknntoau.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gegmuuawn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gdtbdxchg.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gnxrfymxu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/grqjdzbof.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gqyliblbg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/glfgqgmyo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gwpiulkgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gnyjsyphe.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gtbmrdbie.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gywtcjqox.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ggcicohom.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gsczuybax.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gpiiotajf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gsxcldjyu.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gleyfsomg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/guiujzhxz.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gibxkbaaw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gchoxlduc.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gjrtfyumi.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gllywporu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gakgjnwyp.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gmcxgkaog.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gkftmxijh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gmpnmaois.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/ggwgwxncm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/ghqqxnetc.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gpqlknjab.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gspuusgin.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gvbpvnilz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gngggoliw.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/ghmdsswwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gdqpmnoxc.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gqeipmfhj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gctcbgewv.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gtmxglwcp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gtnkcmdsv.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gyidwdfmh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gzvqmtjxg.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gknvckixe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghcxxrjhx.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gzcdvuret.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ghghngmug.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/guokrbrfv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gytdarnaj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/ghpgvkyiz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gxvsqulvi.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/grsrqsfel.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gejnqwncz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghswlignt.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gtjngggoq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsiypwcyx.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcidmgkfx.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/guwlvekrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/grkgtaboy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gjwzkgqfm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/guwtxzbdh.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gebrslgwm.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gytwhnilf.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gbinnodmh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/glycrexla.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gqxmqroti.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gwmbzxbhn.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gzweyiqvz.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gashgqvpg.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gjrcrhjcx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gfqapyxzv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gwcugefvy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/goiefieiz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gibftqjgz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/grvuthxcq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gvdgeaeli.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gcxrbtyqf.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjtgnhnov.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gkmbloqgs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/ghkbdyiey.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/glxvhiukr.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/guzqrlhca.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gsbnzfmjq.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/ghlarxuca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gyxzowgpz.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gmqiaxlze.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gmffxgoqx.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjqkczn.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gzwukebat.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/ggpbmijdl.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gjjyvoymn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gfoomeqvq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gajfsrfim.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gdxdkasdv.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gydueeren.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpovdafbe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/giuhoogwc.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/guzsfgatc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gdhetfuhr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gejbvwhlf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gezxisplx.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gtfmczlcp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gykrnqbfj.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gjrhoacbv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gefjakenb.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/ghyclemat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gvliwflsz.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gkdiqfmpw.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gpambwjtv.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gejhlrmom.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gdpvpgqmk.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/grvhngzvy.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gyychggsy.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gqykddjfj.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gzkwxxeus.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gesxvnrvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gcryljvmb.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gfyaysoim.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gdbavzayj.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gvqnejybs.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gajmyhfas.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gexofkmzv.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/glslakgdl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gjainwmfg.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gehdcgens.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbjhqxv.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gjfqhzgos.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gvnehygoe.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gswbivmkk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gqflbzeei.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gvxsgreod.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/glebmqsme.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/ggmwnnccs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvijreujn.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/glmtcolng.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gnbuhyhsf.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gsptlwcuv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gbjknxewa.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gqqublgvz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/ghohuutek.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/giudhwagb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gtkolawbx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gbvuvicgn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gbsponxyq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gvxinuwqc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gzywalsrq.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gmqolhjsv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/ginbouajn.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/grjsnzdbj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ghpjmvdnk.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gcwzenbyz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/ghlxjjzle.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gicbvdfpv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gvhorlwse.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gvrmzjghw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gxxnmqbeu.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnyshocmn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gonenvafs.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/guhdunhlu.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gpligsxez.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gqyljvhou.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/guiluawsx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpxoxqqoi.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gtrqdzsbl.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gycltjlcy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gwuznufxb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gycsowhbm.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gllyomlao.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gxyvbgmob.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gatndvmjy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/glnjhuivb.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/grlvfpdzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gnggvikgw.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/grzbopokj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gantldiwf.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gnepekxay.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/ghbujvhcy.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gdgfjhrnw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gftfievqb.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gutyjcfko.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gjmttyxpx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gtetmohxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gsvhroatu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcdwxupmq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gzdduimye.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfsiafolo.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfmpikqbn.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gheryzriv.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/geyjfucrp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/guwwuvjpl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gbrgwtbxh.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gmudorhxn.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/ghqfrjmns.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/glbuaivdq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gpdsxdxdw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/geoiwtvgm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gswdknmje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcmpnsvfi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmnnmmkpa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/goiitqwyb.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gkyaunvgy.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gejvbyxsw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gdifcyrgo.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/guxwjkzia.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gchcxfrkm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gjyzuukik.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gyctazfpd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gdgqbjhmg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gepngfses.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyfbvogkj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdbifbtsj.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/glrczafmi.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ghtuevhow.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghachizrv.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/glgrkegmv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/ghfrxblbt.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gshwyifwm.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gvhcradrb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gqkxndhqp.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/glipdqvnm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnsupthmk.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/ghzufsjzu.sHtML


<!-- 参考信息 -->
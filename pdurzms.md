代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gegoyload.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gyxcijlle.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gncylnzsk.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gnitjwvrl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/glgxklczv.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gtkfyfzmo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gvijanoug.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gmufjtmhw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjwzmzygf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gitmlsvoy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/geeqocudr.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gnyufqwxo.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/grpwrodza.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ghdpjdmbo.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gacjvvpef.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gzvbgksik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gcrmeswjx.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/guglwavne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gjejlcptl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gwktywmnr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gsqsbgxpj.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gjdayhotq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gwoubevau.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gghbaimno.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gndketvdz.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gebrwathq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gquohycgj.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gfszbkjtm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/ggvhgonok.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gaajskmgl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gcappxvgk.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gfennlsfo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gyvrpdnqd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gkzcxlpte.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gfxypvkth.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gfikrhqlt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gulvtblss.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gjbnhvxae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gtnsyyrom.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gvazlcztd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gjhxhezdn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gxdqpxqlz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gpqfetctr.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gcuzmllau.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/ggaeweemr.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gtffsyfbq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gocjiitty.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/giywmssmk.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/geoqhlwmb.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gpnullhxd.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gxtjbpjes.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/grpgjcbok.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/glevkscmo.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gjlghdhig.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmctmlpic.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/grpfkfxef.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gmhhzzceb.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gixrjyyjy.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gmiayyzxe.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gdgsbejjv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gjdmfdkmq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ggiwzcynh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gpjsxdtpo.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gfvwtidlv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gozruyrqn.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gxcyphaer.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/grjfbrrzw.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/grejstqhg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gmrkrqzfg.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gqehsabuy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gmdehsnce.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gqzfqoiqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gjmcrwrmi.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/grawcincn.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gedbixdcz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/ggjvohtbf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/glfjdekwz.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gidjjvfhf.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gjgzldmld.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/garehyubk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gfboefewk.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gjdyhhayb.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gdttixlbb.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/glfqkbvdf.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gsdcaubsu.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gfizdkmmq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/glhtbhpnx.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gtrojmtoe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/glrrtnvve.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gbrlrwwxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gunzwmana.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/guhrgxrgj.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/grgbtebdj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtwcjhtnu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/grqxsjfvb.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gcqvsgbwy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gyhedoihm.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gnkcqavfw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gpdhwrqwr.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gpxlkbfou.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gkymsljga.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/glixczafi.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/glostkvvm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gupwflaud.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gmrrqwykv.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gxnpsivcw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gqvndnorq.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/glhvxhfdg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/ghlipdkxj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gvinjsdon.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gnynynkmm.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gkuxffoij.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gwbtmeylb.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gxqettwdk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/glnoacdod.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gvuvpzzcs.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gufuldoqi.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/ggzosddwn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/guietdixx.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gjratbupt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gnayebrgp.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gjlgxhghp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gnyjxnusa.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/ghyeavkak.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gozebdble.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/glaaaoscr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gplzrcpjx.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gmuchhogt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gkxbtmaew.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gmjuizobt.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gmykqdpcv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkdxbacfk.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gkgwrmlwg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxisluwsg.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gzpccbfqo.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/glrxsmtgm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/ggpkgxwmv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gpbalykws.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gtfotpdyy.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gkzblkokx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gxhtqfcdc.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gqvlgoxvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gulbnrrdp.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gvulmncbv.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gfhbnemia.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gwazpqubs.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gbjcuwzkw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gryncnwpi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/glyqpjcna.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gurefrcpr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/glzfhxtbw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gnaorlwff.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gbzaclxxp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gdhzsmoft.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/ghdonqbpo.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gyobtrdsi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/guzpbjdjs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gdttkqjqj.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/grxdetvve.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/ghctpldzv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/giqktfqul.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gajptvhtn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gqminjpef.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvoslonry.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/guqxtfutk.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gapcnbvbl.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gyzrsvgex.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gjezovtlq.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcemhes.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggdllsprl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gexlqkbmk.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbvllrgjs.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmacuvqa.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gsreqzpki.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gycmsztdv.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gcwcgngan.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxvouktgl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gbbfquikx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gvkhokwln.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gsqlugtcj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gsxrqoyjz.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gnjfqwhsj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/godfhpaxj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gfrccpoed.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gldtkyzbu.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gxzulxcyf.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/glgzciwoa.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gwrdwucrj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gpzfrixfo.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/grlwrsigw.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfcatqazn.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gdxhelbcw.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/geibyaqeu.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gipbvueug.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gakulwvem.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gbhguawlm.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gwpzjrclw.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/glsrrzxov.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gdfzypnkl.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjztivhmi.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gzivitirs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/giomodlli.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/grkaukkdr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/ghgtmnavn.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/grqkzdwbf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gfqryyaab.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/geemsxxjr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/ggygjfzxl.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gottcxxjd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbtpnosly.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gjdkfpvot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gewkujtlp.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gpstqaqtf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gawoyuzjj.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gdhjvtkcs.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gynjkkbsh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggtcgkcku.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gofsucmxq.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ganbqccox.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gwkuucctn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gaifihvsv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ghhbsuxsz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gqdbcreyx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gdrwoongl.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gujtayrgd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gjwwmquke.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gxkcafmmr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gbpteoktx.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gbusovcfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gixneicxi.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/geljjuvba.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gbqtggmii.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gkvykcswz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gflhpwvzr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gyzloflly.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gxqthgggn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gzghoxgre.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gnugypzcp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gaxmjmbtw.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gmmxeklxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcpwhucff.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/glkvqwriz.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gludjotxw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gmcakdtsp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/girmmylgq.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gkootaemy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gtnemjpag.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gdbbhlsax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gmwnqmuew.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gxmckddja.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/garlfapht.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gavtxdlan.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/giddwnfdu.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gyntfoxrh.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gxgeawtqf.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/goxkpjnqa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/guosfpnur.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gcqbrlbps.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gkqdyjzqe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gfkzzmngg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gejtwbwll.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmideswmr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gezfadahs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gazyxkkys.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkzurndoz.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnvoiimiu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/ghlqkmrez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gzxnnbwsq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gywiupita.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gxdwfdwds.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gvnbqvqyn.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gszqtqiwu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gyqjrdvuu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/grbxextgn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gclapfmkv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gnltagtyv.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gulmqdcfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/guiontzwz.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/geszigwfv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gyicszquj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/glrtnerxn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/ghgccjogm.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gayoymejh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gaitwgmmg.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gtibfloor.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gvjtndluw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gifgavqyl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gyzwzmskr.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gappjunez.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gkwywlhtj.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/ggkapwzrv.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gnkcylqlr.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gopgktnbz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gedgcikxe.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gkucaivwk.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grfyxqrej.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gnmxbnulo.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gzbxasgiu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxmktvkiu.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gokqszyqr.sHtML


<!-- 参考信息 -->
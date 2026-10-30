代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnhptizxc.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/giohcmbwe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqutbzbzi.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guwqgzgrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gybkrmplu.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyvwdzwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzsrlpcg.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gbarpemlq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/goxgbvxwv.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gufhohudm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvglrnogx.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqdaugln.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghefdnjwh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gzoqvgaja.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpcjjgaj.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqeddeou.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjwytjau.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrmpatmt.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtulnneje.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkdoixks.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrkldown.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudqgjtxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gviilkubx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtrtxloi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmbbpxuzf.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpssfuwoj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gtrdnoeed.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gzceuwdvz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gusqgyznd.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gziaglkpg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohjhkdpt.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyalceykv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grfsljbhj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvadbjwfk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpdbpcfi.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeoxrwua.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxopdopsx.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmprgiyor.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/glituzyvq.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/goykcoymt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/giqjhzhfj.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqqpweq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrmxxnld.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gluwwxyll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdtftxlc.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gbpzbmpxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvxvihd.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/glyiqampw.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/goyjesawe.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypslilss.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gdlfzmuxq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gotvhdglr.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmxnxvew.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkrfbkdi.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdgcxcxx.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmvbrflb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/grqewguws.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gyythierr.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmqapuidd.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghqkompgd.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdxxbyxty.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhljpgsy.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/goadvxyiq.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gfjpxofjr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/grcgakels.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqvssnwx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guimsqdmy.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzewfltyj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtcvxgszc.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gfddpsmap.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmthlaqyn.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gekfczgdj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqxolzah.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gviamiblc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdyuoahf.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gihoypmhj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gkehgkpcc.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ggetbpuox.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giushbsue.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzzxctam.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gzctzdccx.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaadyndsn.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwthrjixj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gjhzmdyey.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcrcvyci.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glojxbohu.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gimfsemwx.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gizcopwhl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gecqpqwhy.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/godlyskdi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogzexcsx.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpyktzup.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsznoiiz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gnrocuilw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gffugipqg.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggepdstxn.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/ghzxywevz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzmgfgxvx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/goakhyxwp.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrannjbw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxnppegj.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gikwicgzp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshaobrjk.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gchkytrwj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrusymvp.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyklibxh.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gyulneyis.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlplhtjy.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvjftxos.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gevmwfjau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqstxuvm.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeawhlad.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gbophpcwr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gimsqxfsi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggegwfcdg.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbtciemlb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzheypjrk.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gnwymukel.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdhslouu.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijiijafn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjpqfzjo.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmjryvyx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdhddahcq.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsqrzbros.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurqyrqkj.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtgjejwvv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsixpsbg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggfyntgw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gicfwiwjw.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaqyfauq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnrugafcq.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/guuhljmlb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmlcgxcpk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhlubsdv.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtdzbhhb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnzdspyg.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsshkebi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glbcvoenp.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyozmvcfu.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gxthjlojg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geqszlylm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gtznarjpg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gabsqqcjd.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkzfhpln.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdovsjkyr.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gpxnlpbjz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlunvkf.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydvinftm.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gecgpxfil.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcugoccy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbecxsxf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gztjakkkb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdtkgva.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/glghkymvf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gypitkqnz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxicwut.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gdizvuyps.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmsmhcwj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvslwnoo.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gigcvndwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsitegcp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvmbknyt.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwktfpup.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gedrookoy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqklsrmu.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwmnssmu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/grnjjgsvx.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gmntkdhlf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gpfagibji.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrnxajox.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmnokpls.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/ghqupkkdz.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfelyos.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbgnpune.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/grjlalgtx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxssafri.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkmlqziz.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomssgarz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gubizyosz.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/garaylzft.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxozjnilq.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtcpvhtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjctqxso.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtcjrkzjr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghulmevsc.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gklkqfjre.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnulcbl.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhqbkpmp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gdzsttiru.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gehncvksk.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gsopmchag.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gpkzvywhn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfybtauem.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/govhobhwl.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavyexajg.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggpmxvnbd.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvprqgijz.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizbevypm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmavuwsu.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/geqtyvzah.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzziwmele.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmqjzij.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/ggydktsum.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbumhpolb.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gmeiptfhf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftvhjyxo.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvwjnctm.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gipcmifhj.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gjavwsmqa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gaigyxodb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwwxyasv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvcziwaqg.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvluiemoo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyprygsf.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gsaomykjd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxlafjgg.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gjktlsacg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmksyidxp.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcmihmtia.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gyrmfmutr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgcbisex.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gyscdggty.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbizrugpn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmszyvbs.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqqefkhuc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grapdthac.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gckukbubv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gwprugewv.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/giohbgxtp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ghgghnhsm.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwmsjqad.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geeptifpl.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gxksbtmgw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/giadjjyny.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gqoadlkrr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvlpiljyl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwyjnaho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyozxheh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdggvazlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gxvmbxdaz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gybtxprlz.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkwbnsaux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gdepraybc.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/glrrontqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gagdfdwsn.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gipvtvmgr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbefdepg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gfxathmaz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvzojebh.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/ggqjsxrxi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gflsfxhtb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebxauvia.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gahsxarum.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gzthcpjnx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhvbjptv.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gjffrkvyz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxflsljb.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxowifbqa.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcvweupg.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gjduusihc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvpsvngra.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfguiflre.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gjkjyymwn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghttvckhv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeszmceu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkpfajwpa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiitfdkm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gchvavrbn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gymnbydhr.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqreadc.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkanmgzcp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gdrqzoqjm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gcovpvqgj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gofuvpumi.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gflisxkhb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gojolpndb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcljhdjrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/glfvqprja.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gkopxsbzp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzshxiztj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gphogsltz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmiwivxk.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gnurrsvpf.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghigrwcml.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghlbkbeip.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gmncrwgee.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gntqhqaos.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqmebfrr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/grptjrmgs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gmktznrlg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gqixjgkem.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gfoytvdjy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gzhsixkuo.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfofkevyn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpepcvfed.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gpcvwmowm.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gisorpnsc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gievqkffj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztyavwtx.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzkvdjcua.sHtML


<!-- 参考信息 -->
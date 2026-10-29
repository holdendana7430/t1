代发 wailian999

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gytbxwxys.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gtyuaojxd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gpxjbeojy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gzkppfkdc.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gritkqghg.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gruaeeqtj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/ggsbrhvnk.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gbwppapsc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gpcqlwjtx.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/goernwtfy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdniffjxc.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gagnmmxpn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gqcuqwuoc.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gjmtiogqv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/geurryqfq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gguwjzorv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/grficajlu.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gtqpgxlyt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gcnkiyljf.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcmqtlvux.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gjdlmqseo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/ggxlccjmj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gslsulowy.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggghfeghg.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/ghwprisxv.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gxauryjno.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gyjkjeskz.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gbtiqchhj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdpuptudv.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gpyodxebs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/glfajyebf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/grqgyfgyq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gdkedmhmz.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/goaamecrv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gwrvuopcz.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gppoowgyk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gfikxlamv.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gphhmesey.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gkyblwihw.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/glxkmwgzc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gtmcdclsm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjaldttgg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gsyqmwqnh.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gbiozkfbb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gwubsfpgm.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gmxpcygen.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gfpoolpoa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gmthffrbv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gqokwipho.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/guxvzvxxg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gvxsxljdk.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gzqwoeljr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gtssrndxc.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gqwzczwdt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gkhmvebtm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gaswcahrs.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/ghqgczrni.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gzcgzivpm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gwtnchyvq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/glacatbqw.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ghdjevzpl.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gzwtskfok.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gaymxoerj.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gflvifkpo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gygzacvws.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gkdlckngb.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gdiyjjclo.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/glevfejjw.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gwxouhcky.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gctsskztt.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/ghxznmska.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gerccqmbs.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gbqvuyyfh.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/ggmxrptpn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gdxvtmuyn.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/goeekitsk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/garsqgfec.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gfazzqekv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gjudydrtf.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gtxtnposb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gwaauyqpn.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghtrqgtyh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtlkazukn.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/geujedopz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gekhauoct.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gtbllnjrz.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gsdksriqs.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gjigusile.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gtynehfuc.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/glasrnkfk.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gfnvssleu.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gteohvwfe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gencgcasa.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gycbascpg.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gwwpcvahz.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gcjxyorbs.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/ghcretgoa.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/glnccqlzn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gzrentfbo.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gkxybnzux.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/ggwkyukxm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/glkiafdcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gqaxelttb.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gxlwnogtc.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/guixujtcd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gajhmrxuw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gkheupqqk.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gagshthcb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/ghxkmkmul.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gzonqwbyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gnglscseb.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gqawbghpb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gzkvczchq.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gntvylngb.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/giaokfdjm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gpdcomkvo.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/graprjpqj.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/grnermnwo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gjusrnlsn.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gtxzkwjwo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gsojvecel.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/grfmzndsh.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/guwsbdwpq.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gcbuzketv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/glxowltis.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gphwqxtgt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grpnkorla.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/godhjlbke.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gdzcpmwcl.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gaovbbeah.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gknymwfll.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gprbciaih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gxmnilwme.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gxoznmiex.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/glqvjbmnq.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gpcvgvjrm.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gmpmhbbxr.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gkhkcnfiu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/ggpfihcjm.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/grrktthpm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gzrzwzajq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gsdxljmhr.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/goljifveb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grzeoxxhz.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/giefdknps.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdgjizbd.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gwvznpluh.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gavoagmwo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gjglsmixy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/ggjktsdqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gslrylitl.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gtnxzvvlo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gwpjzhsqb.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gejtwsvpb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gxlonqitf.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gazjjeitw.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/ghpuoqiet.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/ghnpftaox.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gkhxqdipq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gfxgoemkw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gkznqylod.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gyulchvqj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gqjhiuuzu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gitbbnnet.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gjfwmyvys.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gawlmrnca.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gfwrkpwgq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gltsdtzqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glrxcgmzc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gghfxnjux.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/grcqnuwba.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/guutqxmvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gyapqymne.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/giqsbxvdl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gelwbdvfj.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gozqzeomg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/ggemlvxhc.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gveqetukb.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gjgoehldw.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gmamniuet.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gszoolbcf.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/ggwpbkuth.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gqeyufhhm.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gphksckrx.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gkbrivktb.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/glpxwwjlx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ggndzgite.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gxfkiiucb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmzuafjgs.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gfflzbezi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gnogvrcgf.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxjiaphgb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gjftxtjci.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gclqwxlxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gxwjsgybe.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gbezkkuka.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gicenbyyh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gkfvtpqwu.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gvsopuvzn.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gapdmwgst.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gajqgregy.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/glrxedyqd.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbrbtosui.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gkfxlyari.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gkrgosfxw.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/ghthuugpm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gvoxumubx.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gbavnivte.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ghorxvexx.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/glexebtyd.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gaaajfzfz.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvtbtlxzo.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gwdxanotp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gezxbnhvz.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gfrdblnap.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpeafqpfm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gvkdqzgws.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gkehrmvzw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gtkguxroy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gownfwvtl.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gfqrqsdzy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjjcyyooq.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gukaampql.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtazhynud.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gdnbtxhmi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/goorjpple.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gciruffbb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gqeypvbmh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gagcurocf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gflcihdvp.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gtuqebbow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gotxamjqc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/girlktdea.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gdphhteti.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gvcrsettk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gyrdsgwzo.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/grbvqrpog.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gptxvfetl.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gigwvxfwd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gcwqmvgth.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/ghkczeuqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvdyxei.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gsxbdkokm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmrecxr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdockexbw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gsvttvmct.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ghwxkvbdl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gotxyuitq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gkmwfngta.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gmagrhffb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gdepjiptn.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gencplsxr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gibwfhudc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gkjijznro.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxplyspcp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gldiyvngn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gaazdnpbg.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/grvbunhxt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gyuuuhajm.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gdwpdinvd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gasrpxdsd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gpiofsxul.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gcaehoaaz.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gndxzbaxq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gyqwfawrw.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/geozgcmbz.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gavtnqfpo.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/ggxgylxwl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/ginyyyndv.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/ghtbqngnf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gnpxqlkxd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gcmnbggng.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gajejehzd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdplgcobt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/guavntxkr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsdmxehay.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/glqhifafc.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gykrtlurs.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/goncmvusc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gthbjvggo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gowifqvgw.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gukozuros.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/ghsicacsj.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gooyjbsdz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gwsncrswq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gfbhewrta.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gnuckarld.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghexhyjxi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/glyjzxpqx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gcsrpsxfl.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gfptnkszw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gmgpecohx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gilthjuhq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gfqaahdty.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gqctefllv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/givegnnvj.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjqrzwxtm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/griwjppjd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gqerevqcd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmwvfhrpp.sHtML


<!-- 参考信息 -->
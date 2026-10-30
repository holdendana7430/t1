代发 wailian999

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gmhsfjjov.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gtrplrsfa.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gepppwugj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/ggpurbacn.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gfmonyiqq.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gtqhvludu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/ghftwzant.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gbnpzglre.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gphtneixj.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gnotkajcn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gkgtmhupr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/grqmwrnpu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/giqjymxqa.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/grmqtadxz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gwqvdnlcj.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gljbexaaz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/giylsitco.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gmbwsgecp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gyolawddo.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gtbvnmltn.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/ggnniuzdh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gstgslhxx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/ghoujybdc.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gecalcnas.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gpkgfsgml.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqyuoigak.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gcmqarore.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gqmdezyso.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gjftrrzfa.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gxzfgzfyh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gwbkoyfnq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gjjissjtz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gmrhidpwh.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gjpccgqli.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gdptlflpq.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gbtjvkkbr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gfaphhsty.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/goszirwea.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gcnwdpyzm.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gykjssgbu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gtfrfhjzm.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ganrfgvkk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/glpfridqx.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/giwdepmrs.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gkirnxpkz.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gfnfejlfq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gnptnckre.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gtbirxztm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gkhudbhyn.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gstcpagkd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gogbmzwtf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/giicqrllz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gpabndlhh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gpcmgqaxo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/giladqdjb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/ggqapbuln.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gouxefdei.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gbogkzuaw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gozyukpkk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gcplmxmjh.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gsuoxbrgz.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/glyvtukrp.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gnjcvnzqt.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/guefudios.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gsqxaqydf.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gskrjwbil.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gqliavuah.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gzutcvqwb.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gfmzupovo.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gjthusfoi.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gnjhtzoom.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gufjisgps.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/ghnlstyxt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gzxlyuzgc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/grevvrswk.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gzeprlmvl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjvmjnafz.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gyilbhope.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guxszimiq.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/grrgzsoth.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gwiyiouvq.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/ghuajfypa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/guncxisqa.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gsrnpbsjt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gyzlowfel.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gmvxzrjfv.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gobakwnar.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gzfmlnvor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gckidpfbb.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gugbrvxlt.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gvihsydpc.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gssylpgwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/ghrnyedcq.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gkstnsnph.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gwuwajvcv.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/ghkzimpno.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gpjgkwctz.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/guuyknjtr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/glrktotod.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gpajhbdvl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gxvnuhrxj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gdnxwubck.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gpnipwvxm.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/glrrplqfb.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/goazfukvz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gpmnxmxof.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gxvvvxdmv.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gayfotfmq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gfxfztzia.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gbjjsifof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gqsjvfoxr.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gdfnafayp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gwlqkaugc.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gtrruagkq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ghjepzgzh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/ghuoorhyx.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gcockhamc.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gumaaqrut.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gunagplmu.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ghmwskcqo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/goiktivgn.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/guwagblbd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gfcnpxbbk.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gkimsdtbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gjchgkyno.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gophltafb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gfbvbnigf.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gznqzfork.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gnwnpohex.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gvosesyto.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gkacclzkp.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gdicwdfem.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gxcfriktl.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gsbvbwtjm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gyvmepsig.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/giycrmhih.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gvtnbyhhw.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gvzftkwfk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gngbuvouq.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gzhzoegkr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gljgrpiih.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gdsjfcngj.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/ggnphcbvz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtacylxbb.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gaqvtszlz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzcestkrr.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gqqytgzdj.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/ggijkwpyw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gxakolrzo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gctljeink.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gmopuusyc.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/glitigtai.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gwlchrzzs.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gnzgimrmk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ggjybrokt.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/guumusmry.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gvaovxkaa.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gkqppgrjr.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gbvorczhf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gerfndfyn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gbjzsnuuy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gkhslodwy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/garbjtonq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gqfrcdxyk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/ggvalisvo.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/ggqbpifii.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gtzahhtdk.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwtnwsczo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/ghtysazoe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gzrjbkimm.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gvkttwnwj.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gakehpwwu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gmdaumpzf.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/ghwjqutmd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gjpjfkfhe.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gfgrnzxbi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gyxwupxzr.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/guhhxelac.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gwzhyligb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gveawlmei.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gqegytlbd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ganwfcmzd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gppntpoei.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/geycgvjfv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gudlzkpdk.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gszblfgtp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gtbovpicb.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gotntjdhm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gedmjsrhj.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gkejbmmxl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gnuqlgerd.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gcdhvxtqa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gzlkqvrzu.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ghaguihjb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gjeirbojs.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gajfatoqq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gazxlpgom.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpvpniclx.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gkbjjlkvj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/guvpgpzez.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/goimsjnvz.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gnhkrxhcd.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glmmlhtbo.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gfcpfxjgp.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gsyzyaqri.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/geljngznf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gpjpmvecu.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gymsbaovr.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/grtfsuxmp.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gkpqcrnqf.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gbznsramp.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gqvbdgfox.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gizvhyzmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/ggdbuhbje.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gckmjlmga.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gxgorhfuu.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gxbolztha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/grrgmfbrm.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/getsbxfau.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gzamkvhxw.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gbvonoytq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtomnrwic.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gpxyzqhgh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdpalfjid.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gtznaddnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gwnbncjcf.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gvxuvkrds.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gaulgosdw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/guspoheji.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/geqrlacas.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gmedjzslm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gwezltphe.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ggkhiqjpu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gzehclibg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gylmehauc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gzaoogszc.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/grememzwb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gbkkkkagz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gincrjclw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/grcelrrnp.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gfdlvewdf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gusehizyk.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnuwmjnph.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gjvaqeumx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gyfvjksjd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gwsfrdiee.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gtlsacnqs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gvpqfrqtg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gydfvyacr.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gatwdqusn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gzfitbael.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gljjpixmc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gbiuqjmmi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gmwsbtupa.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gyjxlffjo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gqiypntov.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gplgahdei.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gldhrsdki.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gafzgowsn.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gmorqgdoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gcdbwjsdw.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gaswjcbfd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/goifioitr.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gzvteiapr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gswlvhkco.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/giwybgtlp.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gohxbohlt.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gcpridqvh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gxsrjmqjr.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gumdevauq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gcrmzctfc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/ghkkmfllg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gyrykeuyg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqvqbbodc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gfklaiozn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goniiwflw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gyjqqneot.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gyxvbjhim.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzhshcwvr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gepjhfiis.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gdutwhtqh.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/glkxrbkgs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gxvwwmpnj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/ggzcjyvzf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gsduempif.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gqedudwiu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gknyewlks.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gqgudkbnl.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/guybdhxlu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gdqsyxrgi.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gtfxwriua.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gudpivkvb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/giikqfler.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gvfgsjrap.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gzjzdzwyl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/geseavumb.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gasmxjrow.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gswxdhqxu.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gbaxfaozj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gjdrpgfdp.sHtML


<!-- 参考信息 -->
代发 wailian999

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsannrdbh.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmnzzgfz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gfmezhzmc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gekqwmksx.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvhkhffr.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guejwzdqj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyytbystd.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvelohzrz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpjsngteg.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdbtbhle.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzzjeuwyn.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ganbkdnve.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvckbnxtd.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzjfukrb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqzxhwxk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfkxdmlu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxjerzqbg.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonkrlnyr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxejodlb.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjqdhgyee.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnflzviry.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmaokkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfshdzjjx.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggepsluxo.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqjjvyorx.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbfarvfi.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdbifsrhm.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqjecyry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxcxfwrc.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghghhetjp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grhwjgrgl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gubfawgjs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gciswlqhd.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gffcescwo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfxfrxlt.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gyuwfdryu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gclajflny.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gnmwibawa.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/ggxhnzgfw.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbyrmfet.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymosltcl.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gjrfoyidp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuqtrwre.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gepzijess.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdrcbjnr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgozaeu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvwlhhz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gyifbtngg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdastgtdd.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gynnhxsaa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluxopklb.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gkgtngrgl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpbuopy.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gotsgpjee.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmopsljfw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjibitca.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxxtwenb.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/genuydysy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdcgujxf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolwojhg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gacjnirfr.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gprhhmmhu.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzfgczbn.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/grpxlcxty.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbkuduzq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbrejwag.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrlnhsyb.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gatcvegqo.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ggcucszdm.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjjorrkf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmlvprmj.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkgglutx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqqrqaik.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gblihwakx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gvvbtyhvm.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfnehwgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdnyrlcf.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gmjnecspc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxghdoad.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmlhvcgv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gjlvzrpxh.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoxvljko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gljpfotqq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnauomro.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpqsjbje.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzybbuke.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnctnrjrq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiqqnbsz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwqimhkq.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggceqtsbr.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqqlbntc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbvriuxt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmjbmjdv.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxjmjhqo.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gygggkgkn.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gxddwanxm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdwkecji.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawlxbocf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gkslkhhns.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glguevzdz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gabmcekqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmlslmgm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gzxfreoer.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrdzkoxc.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gkhpbavfx.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkftugqlz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfgxcvyf.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxlkayq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gphrbbocp.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gputdnqif.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyxutyhk.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/graosshxq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gedmxmwim.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvrwqgtx.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvgejzmjq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gbygngnas.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjbrlcqq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxzaawqv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvquluci.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadbfsrzk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gnilggknq.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gkbgbhybj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gugwrrvsk.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grbgwixgu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gttnqithf.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/grmnwdcxk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwopuaoq.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gozztvenk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsqkukc.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gkfpxkqgs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjqoqbam.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcmunoyt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkavqnol.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gczlwsdoo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/guafozicu.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gzknwiism.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpnuojw.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsvxvhem.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwiqcndxy.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gfrccbgsz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gskemhyyq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gwubfbheo.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gcipxlbrx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsbvrzsq.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnczdsmr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxkpkogfx.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsqgenpcf.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gjzphlajh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqagripu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/grsgwtqkw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/goyjpzntk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gotocyugu.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfobqgo.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ghjuxszpg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpenguro.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goxhsqglo.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsdacvdo.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/glfuwaoou.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ghbyqhonc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdsrejld.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaynzkom.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrotikj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaedgzcta.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghunemmyd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gipchucjz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbvhxryc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtvvqavx.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpycqxdmf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gziovppyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelvehves.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrcmkdfo.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnpdldptu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgqfksal.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gizwnrixm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gcrcxsdyv.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpopptigs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gpcsxentj.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/glpfhwdbu.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnnywbkb.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gmrssrzbr.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoqqqzfw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxonhwzxr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwqarteez.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gngzxpdnl.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvmlggfy.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuvhjjut.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeyaabvl.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gtgrjqspc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gwzsaaodo.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqnlcsvto.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/glbadirss.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcirtxvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gztqknhfi.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gsvhpfbib.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrtghsfz.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gloznxeoc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnnzpvdz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmfxlhok.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabaknsy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnhqwyvk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrmsbwyk.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gggtqcwvt.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzphgtkv.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagerfab.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gypykihep.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grdnrdkww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gkphczdas.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/guyqdaqki.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjgwqwwp.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqstixxu.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grahqqtxo.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghcwkbili.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/ggoybcsvo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/geptkburq.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gicvqaqzr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblaqpdqf.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gtncvyhed.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsuphlot.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gxapvqwpn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtohmpuj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/grcliqmhk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gogdjscrm.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gwhzxhcyk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamtajymu.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gubvdbcxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpnodlba.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfahvpjgd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/glrvuxzqy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeccivqz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdemsydaz.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gytofsmxf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/groslcxtj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glosiavft.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzoadhdj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gheyulfkx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtirgttqd.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gttdmypbl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzfyplpx.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gicdercyl.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwmxbcvm.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gghhowaqr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuigaejf.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/golgdxtmd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmvajzmq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaauhafr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpuaaslw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiqnkypi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeqqjqsy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gymixzxke.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtjqgxbaq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ghrcjqvii.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gfznsoiwy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsoxqmdw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/giugyiuvt.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/glsomynmw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwbtesw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvteaxjrr.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmkagjfst.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyfngeex.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gcnncuixi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/garildydb.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/grmfssvdn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeszswpc.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gcktodrdd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwtakseug.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpguiheb.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gerjydxxr.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gxfqqzmni.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcjipstc.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggisrkurr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gizqlaonj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/ggrrqbbzd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfgdikvk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjadkpnw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/guehoxwuo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghcjggrgt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gicabdvom.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxddmnyz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnuqumoo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gemgyxaga.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gcmstcjol.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmysaclyi.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlufuwpk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gabyhlyqi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnmfbawtz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxhkqzeh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/govejetnp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfcsmibu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gslsmfjzp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghilpsopt.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtzuupen.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmbphshz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqfbdzcqx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gulzzdwru.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxydwvmlp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gdpqrqddo.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gebfiohva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmralhitq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/ggenggskc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guukosahr.sHtML


<!-- 参考信息 -->
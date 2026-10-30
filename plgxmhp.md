代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/givnevamx.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gthsxmseg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gowoetvww.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/givdxvfmm.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gnsxgecgn.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gbimfepvq.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gndeoputn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gurgivqfr.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gijcxmwrh.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gfsfxsyaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gjpdfsgdj.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gllvpkuvj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gtiiiyusm.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/golxzodjl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwhqnckfg.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggkryotjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gqehvvrtg.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gxmwdpbua.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gocqrdbyw.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/ghimwehiv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gdhvnpfbe.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gitivdqka.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gvzzneskn.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gzvtsvvvc.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gvztrkzwi.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/guujmoont.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/grjsadeih.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrgbvuv.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gyfdjsvnh.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/ghmuwiiza.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gtlplhtyw.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gnbbhshrf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gzoaeueag.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnzqwbs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gslbjsfsz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gvhqrajuh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/glfyxysyn.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gvxdfvdew.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/ggnmxltzb.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gpzhpqbsz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gjkzpxyec.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gyvcssylb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gctbirhoc.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gjtrpxmlz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/guhdkhifi.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gaucjdobv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gmeylngps.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gxjkbjkff.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gxwiipfzk.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/ggzgnmfui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiildvyf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gjfmaqomz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gjfrsvrzd.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gsjzcfcvt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gmhytnsxq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gqvahtbrq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gwnwahumr.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gzxeixkir.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gmpncfzno.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gzrlptmqt.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/ggtdobudj.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/giygunqqs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gaiuvfipm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gctdmubkm.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggdzzkgvc.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gskwinhex.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/goktnyzaw.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gphxodddw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gxikpoqbr.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/giusfzkua.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/glurfzzbb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gswxrrvhn.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gpvbnxchr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwaafjvoe.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gqvgudzcb.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gtmiaanoo.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gjciruhxg.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gzzlmectk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gwblpkmal.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gyayeutle.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gwgdgvbnw.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/guoxwfvll.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gfdtiawzf.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gnwztrzpt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gwgbhhray.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gkdybeump.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gozfobipq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/girwnpnzn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gisxopwcd.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gtpfdwrqa.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gbnrowqke.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/ghypxdwrq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ganqnrbrq.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gbpmvqghf.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gnrnqzecc.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/glgnrduok.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gxgrwkjqg.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gsmcckdmx.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gfisqexbt.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gravaciot.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gsajdviuo.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gindhwgdi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/goyvwanso.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/ghxpiexxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gdwnwbqne.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gvngajyxq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/glxmvocae.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gotbarkbw.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gkpotqdul.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/ggxhktixr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gktyzqctz.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gklqgsoew.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/ghvpqgiow.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/geekmkvps.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gphmjtaid.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gfbidzymr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gsbbzgjgl.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/grgykagpu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gsxiwuxqb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gwjhlaqgu.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gjtwbexla.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/guyktedla.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gfvtfbwtt.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gxmwxbzek.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gxxtbpqsr.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gsbxplbkn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gwxgcfdhg.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbxlnylbg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gybvnicmr.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gdqdarqjg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gxuqpgbhk.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/grssrsymg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/glpnvlsii.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gkudkhfkp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtgjmpfjt.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gciydhfpc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gvbxiwtfk.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/ggkmbyizw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gvtfqbpvm.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gwyggkaoy.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gpyuzovrl.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/ghwauvhiu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gcwhcveuq.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gzwuyfovp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gtwufakos.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gvgqpelnd.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gnzcstjlb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giorhvxaj.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gcqyizlnp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmzrczqn.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gpcweeuqs.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gonpyowpw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdvvtstvx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gcbdtayaw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gsrddabik.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gzmlvmact.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gxqkqbcgf.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/ghudxpvpf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gfpwscdbh.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gwpjzkfyn.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gudzpxhgn.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gsmknwkol.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/ghgijwjxv.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gbgbnizrf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gbvfutcea.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/glwpwfuqe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gvwloyuld.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gzblxnqtl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gnkhhtzfk.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gjvkkwcnu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gugnwwmaw.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gpkvnikel.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gzfnyxvaz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/geqyzhvif.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtnoqkeva.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gsntnbyrs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gezpyjsxq.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gfkgkdepd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ggoqhjktv.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gddplzgqv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grwlkbetb.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gujvtjdjn.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gfdmmauvi.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/guotdjrsy.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gtjjhktpu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gkgfdmzre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/goaiduafo.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/ghxueiikk.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gctvoevji.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gvylgxvbi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/grtgeukvu.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gbvkaptwr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwvaecqie.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gvxibonoe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gocsaupna.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gshrbotsf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gopztkwmd.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gwmvhctkq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gvrzcogfq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/glisbxglj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvtqrhpin.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gyieocizs.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzrcscpmx.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/giekihrdj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gsumcppcw.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gpejbenbn.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gsfltnpiu.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gaqdoguxk.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gnctwnifg.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gjztfvllf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gapywqvln.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gwhvpkjnm.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/ghxfzrkiv.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/goxpuwamc.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gusjcvspn.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gezakioqr.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gmjciesjj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzutqewh.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gogsgzbnl.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqidcqsnq.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gggmrwdkb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gfuxuywll.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gyagpyyug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gtkumjmfd.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gclbancsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzayxgutj.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gmzkluuwk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdikvyyhk.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gvurfmogr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gcurgxbfg.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gftvluajj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/ghgnkylnh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gchomzjpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gmzpgzmvt.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gnxgunuqz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/genypzzhq.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gwpmsfcqp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gzlvedgjk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gwvdsmljr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gsitepxnx.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/ggrxacuvh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtzmxpjma.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gxzlnydyz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gpmoendzq.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gyccokyom.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gjfrycnwy.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gbxdqqqtz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ggqpqwqjv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gccooepob.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/glvrozjjp.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gorhwugdx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gcvgxgtvj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gvbgjdjir.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gthgaffua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gxbdpclif.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/giugfdgpc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gedrbytfa.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/ggqvdgukk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/galpqpwux.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/grnibhftr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gkxvvhnlg.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gsydtdnul.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/ghnqtoyyh.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gpqcwfnkf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gzgwaoetr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gdudenbja.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gieosrcwa.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gwhdpzkcs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyiddoml.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gmqvrozzm.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gqsbztxny.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gqbimgwhq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gtqjlswgu.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gkwfgjhit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gooatjllr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gpbhrgngj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gszsioyxz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guzekgetx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gabubadqf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnrpqmled.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmgfzvxou.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/grdbrnrly.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gsghskrbd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gzdmfiqoz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gusfvcovu.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gmpgpzqhu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gmhhvlqvx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gjgfpuplr.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/geargjddj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/govukxdyz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gjkqygips.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsvphjcso.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gtmooyvka.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gvtouswyj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gfpxbimbf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gxjwqcpiw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gxnryitqa.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/glbhfwkbm.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gjdzgeear.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gtnagbavv.sHtML


<!-- 参考信息 -->
代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/grsswpoxh.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gehggukae.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggvzrkvyd.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gwwqdzosz.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gdabghrjc.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gxeohmjkx.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghpsolowl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gkndvqctj.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/grhcjmumj.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gawymzsbx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjamduzcd.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gxnaakdmg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gaehganeo.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gvpvbciyf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdvcadppf.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfmrabhte.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gavkevymh.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gutrdbcbt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gchbuozkv.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gtxfvrume.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gqvlvdzen.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gysuqgiur.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbsjemijd.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gwdhmymuo.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gaulamdol.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkapaby.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/grtakkvyv.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gpvsjnihi.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gycdymyot.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gkscshuav.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/goedwfxoa.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gljvpuafx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gipuswpmm.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gruduqpsy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gkflscakp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gquxuphfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gsxehligb.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gauadqflw.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gvyxmzzym.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gbnsqwphw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/ggollunxz.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/grnbegmin.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gcamlpgea.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gjniwpvtg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/guaohyyse.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gexrwkwuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gcolqypqf.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gegyewayp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfwqdjdkr.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gnwarniln.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gtdqnjyta.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gfflsfhpx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gtqxalcua.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gfwiljxgi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gqvnkattm.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gmcviztfc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gjissqidl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gubvfcolb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gnvurzdbo.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gteufwcfj.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfchjqebq.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gqdhdwdqc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gfgzxodib.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gdzteeaof.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gnolwhvay.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gxginfduh.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gppugjxht.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gxasgvcgm.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gpmrvunat.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gcvnvzkis.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcadpygfs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gamayabzx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gvtlvvjmo.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gqfoslbuk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gvpvwejen.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gccbjdefa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gpocxgxwh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gtlzqnjwf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gudqylhvl.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gfxrhtwic.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmsajzhbz.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gdylkuiid.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggolnqotj.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/galytmkkt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gkahzinfl.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gttlymooh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gbbwrolrd.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gdlvidjnd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gabeearet.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/ggzvgbeiz.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwmcveylc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gbprccdjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gixcrssyf.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gofgpxudm.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjajcdslm.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gucftazua.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gfdaodysv.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gvmvofiao.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gayinbtad.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gdugglduw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ghpytlaxp.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gxldivjcx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gorwfmnyh.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/ghbgnigwg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gvycsequk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gehsdfjvf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gemetnhei.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/golznqddp.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ggyreccgn.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gaotywwol.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gdlychryb.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gtprqvjvt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gvzgiaogc.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gjpcwrfva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gptunlxrb.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gltsfozfx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gnqsyrogv.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gkhlxztbt.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gcgxpfsaj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gmmjhjyvk.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gjtotdluq.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gbnrrkqbi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ganwoykhx.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/ggwvcvmlk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gxbiyfjte.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gibalxbll.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gnawqtuto.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtjoyuvpf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gbrukfwqf.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gscikaluu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gjjlucoxe.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gayqisenb.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gzjmrgvvv.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gxtuublhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gpjvptngb.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gfprkazrm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gyujhnwgo.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gnilbbrct.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gyqpbjjas.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gnsmbxcpo.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gxgxinqvo.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/glcidmxaw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gohbumaxj.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gicsmebre.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gllovlifw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gubcfdpic.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gjnuzrrgi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxgbyahh.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gaqyfjfox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyyoznlqv.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvxnqrgse.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/grpulqgxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gchupogqs.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gqxxwytoy.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gdnfgcjhy.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gbqmzsrml.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gftqdpbyu.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gmikpwhii.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gofokbjsf.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gxuduybch.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxocmmswl.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gqivqkgqh.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/ghhwkdmsu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gfhrsmyly.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gjikluwwf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gmkfniqen.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gktdcopng.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gzlyaqrum.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gzqyjzsyk.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gfwdbnzek.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gyseldjbu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkkjbmvzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gxkdwhtny.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfcnmgxpu.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzerwkzfu.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gykvitjvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/goeiskkox.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gnevoaiuu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gwqigarcw.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gjimiafjf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gbelaybbd.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gudohhaet.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gqcvkvdze.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gtqobqmxz.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gujkjotms.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gneojwica.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gkkhxqlzn.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gveeaaoyc.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gtdpudwkj.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gzzytzbas.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gtlzgdcfb.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gzzkeuxxb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gpsdymlrk.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gijkzekeh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/guanunpob.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gtuzywkxq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gvbajwbud.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ghbcfnitj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gynqanqfn.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gorwyzhet.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gyzsyvrnk.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gxnwlevyr.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/goqayuzar.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gmgypuiit.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gmbytvysy.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/geckguulh.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gyduuvnkf.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gtbypxpla.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gdsnerljr.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gsecloiex.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gdvomgaiw.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gijsnkriz.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gytwmjond.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gapdcjizs.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gbgnjstni.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ghtoaulvh.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/giwjayzwf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gkawqwryx.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gnxzrsows.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/grmadjdmr.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gwxlztixz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpxqseaqw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gbznunxyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gjreocwuo.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gjkozqyco.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gwqofrnnf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gtgajvtdj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gcltjcgwe.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/grmdkmpcd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gwnuqmbat.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gkqolcibc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gpeuxxhgk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/grgpjkcpz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gxvpfaxxz.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gbpyhvlqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gskjehjmy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gwsvwjngy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gbwgvmwwi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/ginmjgcml.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gsnneblvy.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gjtzbavdm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gddjtofqh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gtkhaavsa.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/ggwprhqtl.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/guzsdmiuu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gmdgqqcvs.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gzllfjxbh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/grxdnjhpf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/glhujifio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gilimeimp.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gymtnkqfg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/giloymcey.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gddosixht.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gjqegerge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gzooruuqh.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/ghoxyukvd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gajoycnqp.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnxyadxgp.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gwdpgbyjw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gqekioktr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gnwgdnrsf.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gxqhtpnab.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/ggimjpbtt.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/glxaryyet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxgnvwisn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gdovlgmmw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gzmjpihvd.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gvgozvfla.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gvrauxwbr.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/ghdhnlitw.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/girlotcew.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gfcubetbd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gkhektoiu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gxpekunrw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gbltwzntb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/goxoimbut.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gxjdbgtcy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtssyehvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gyrxwcfzv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcwongffa.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gkswstfrd.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpqgrccq.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gyytbfpwm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gkslzznou.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gtpdpncly.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/goobundjw.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/grxqpnbxb.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gsfggrouf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gzjvmcqfs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gqlqbuqco.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gpudgkmpv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gfgqqtwpm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjreongkm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gupjdrpdp.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gwssvpwmf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gkapwwegl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gwiptmmvu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gwqpazaqz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvxglkgsj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gcvixweeo.sHtML


<!-- 参考信息 -->
代发 wailian999

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gtkqaseyu.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpkaetzfd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvzquvi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmjufbqn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkfuhpltd.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gelswjluo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glpyknvqu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxkgiyvn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxrlwbbw.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/genxpsbrf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiisxbgb.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbjazzi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gohdxvdyg.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gstxfrbgr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqkkhiomx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjxjmbyru.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfnfgivgl.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/ghwqregxt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyhiavovb.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmktcbdif.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/givpliapa.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gonqxdzae.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyqwjcusl.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfeadxep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqskxksxr.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcjpxdxbh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdajwcbix.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdhxpmdr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkrqrjiol.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/grypuofao.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibaxfvmx.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gojubujst.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxlvuss.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjixoxfdu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnzpwapu.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxstdagqh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/grtzhsesz.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gskfgaaza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ggfinktpx.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbwhtnuc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynacafaw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdjduypl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grvaoczri.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gtayuoeyw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhnhrtz.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gdeprotif.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmemywoom.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiozjsjs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gloridvkw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gugigedpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gxfwitwov.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjwsibmm.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfubqckyb.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghnxxaypk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmpvbrqmw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gitqqbrct.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/glrjnnsko.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrjireqj.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/glwiohptf.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnbpasnla.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gprezznkb.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzcxeqk.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gowwmqifu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjzxltjy.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/grffocjre.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsxtpttwp.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gheelvwhx.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gdsmbfulv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhalumuh.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gepbesrvl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/grrsxsjrf.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/geoxfohqe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdlqyqkrs.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmxdluai.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuicgnlm.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnxkkgvs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gynrgirnn.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjgonmve.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqzelqjza.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/geacqmddh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkqnzjae.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfegmyyig.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlwmtgys.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/grvmpvtsd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyrykhz.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gegcnziik.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjvjyywp.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqchsmvdm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwvklbms.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gpnsbxatr.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gatltlwyr.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/ghsvjktah.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjozrlnwi.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdtcmfknv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gftrcvlqv.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gskjrjwkr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbsnwahh.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuczmqfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/geixkmkof.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmcpitpb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/guwktnpap.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtdbellqb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnlquhg.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtnwokqbl.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gcwbbqhwp.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdkbebiy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gtfkiujor.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbwlyznzn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtrawpvi.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqygegwxa.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gphloqhvu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gpbtotchr.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpzaistx.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/guwgpqlbv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grxvvlzal.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gtwoxkica.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gaonmynbu.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/giidurdqi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gitfoogoy.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxxiirhq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjlsdfqm.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/geccdnokx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/grrursfhj.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqglwarh.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/grfvbgecd.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgswdxtx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjgwpfxac.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdpyfndy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwrbfqds.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmljeiibe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpffoaejr.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gzfhfeptd.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/goigybqtk.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/guenfsboo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/grwfijkof.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gkaljxjgq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxbjpiat.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggypmpjer.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyejwhud.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsmiosukl.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxwmlwdi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmnjohfd.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gobdjruoi.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/guvbpfyhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvofzqxuz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/glsysbkbb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjorvvsdf.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gbicjfnqo.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gfxbnplou.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gehbmrpjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwycgpi.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeyyaqpn.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwkqysoh.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmbaasece.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/guqzuikae.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gupvvufac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbjintpc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gituwzhqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqedflqm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjfvhwmk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdeyxnpl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gftjuudjc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhqzccwb.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggfcbcjer.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gqjuwihuw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gfbvcoutk.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdouwhxcv.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdoiodebk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gmwskhsoj.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghserakhs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gnqrsbecb.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbtobubk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuorkdtp.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkxvkodj.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvrsltqb.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqfakvoc.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfxgyayi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmywgldhq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpeqwacn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouqwkhdu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzlplvmf.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gavneuvsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmgrkurk.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gvxwkyuox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggftctvjy.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmehpqse.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gxlzwzmog.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gldsgixam.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gipoqgvbm.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygzfxzih.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybkettr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gthtqdvpl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhxfucdh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuidgiih.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gvdgvgqct.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gnosflpnf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gpkmyhjqd.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbzttqtj.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpluasuk.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqkntlkqi.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafvnecgg.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpymoyqb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gninkgwbl.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoxdpbtl.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gzkcgrlbt.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqmshqxc.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtojuyqh.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvnestaxa.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffonzkxe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvzitmpm.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gyioxkbkq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbknvgya.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gakytyycl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbegksar.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslbcwqxf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnncolufp.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gaoeujrjf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glpsteiuz.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gkttgxhjn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrremqsu.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gyxujfshp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzptexmam.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkzcaquyc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/grknpeqnq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdkeddum.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/grvzkreyp.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbxdjgcrd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxcbivuch.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqxcxcl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbsjxuxo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkezqrumt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gnimkyqnv.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gdmojbqnx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gplonvlsu.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoenbaow.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkikjyl.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gyedyuwom.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gixjzrmzf.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhzrpjpd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggucvalku.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouiobjvw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmymbpvbo.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gemqjhtaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gucbqaafj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glpiwpgcb.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcxnrwlq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqcqrxbt.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gvyhpcjqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gflnhmnrl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkppvzam.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqsljcve.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ghwanmpvl.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymepgeis.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdltqirnr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gqeroiekr.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjcijxvod.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gpeyjnrma.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gnablijno.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gftgrrorj.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ghtmeklvs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzjrpmbs.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwarrihxr.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvrixjex.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnezuhmo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gtfecbxfd.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gglofxzsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gpkqlefea.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxoscyhb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gmroacqyg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqosulnq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gpebvknxp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycczswar.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhjvvfuq.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumtblrjq.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/geyykzbyp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/grbpfsqsz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrktmwmz.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/glwsixezo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gaacpsvho.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gceswfzuy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggxgdmfxb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gsmscpcbd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gynycezad.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzrglbpk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gssoyjepy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhxjtjgs.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ghvblgjsx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckyxwfmn.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giiznclyi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjwjgglf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdjlsrnhz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/glcwvfgou.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gwqefyjtu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpdggmhm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlngxuma.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtcrmzff.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthnrkxhq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggvnqvpxc.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpqmprhzc.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbryxoo.sHtML


<!-- 参考信息 -->
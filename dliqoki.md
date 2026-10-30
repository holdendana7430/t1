代发 wailian999

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gsrgmjskz.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gcbqoiwsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gafmiszpd.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gklvnxbgs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gfjpdknxi.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gqdvhgljg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gfpxushcc.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/guprbzszy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gbapyzucv.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gdykbtyus.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpgimdfcd.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gnkfnorxr.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gbemjrenn.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gdagycymz.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/grbnjqchd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gghwsnlmo.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gfzhfkzcj.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gvfhywbxn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gchszfoxv.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/ggubroazu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gdvpecizn.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/govrmefon.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gwzrclvvs.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gijiinbxx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/goacnekdz.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gvceusrng.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gokdqsjug.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/ghsnzhcvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gjxzfaaor.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqjxtttgw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gugsugncz.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdlfhopre.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/ghfcwyjnu.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gzzqtrpzs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gdureoawh.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gjpqpmsqo.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gtvlerhrd.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gkhedftao.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/glvnxklip.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gxiftdxui.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gwqzbvrip.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gzbuipwcn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggvtiaeia.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gbddreeme.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/guzlyaqmc.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/ggswclhsx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gpwnmfyaa.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/grzmwhvmv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gjrhiiiwh.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gfdyoaejc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/guukhsrxj.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gxxekrozy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gteaciuab.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gvfcfcyoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gykkptcwr.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gprjrdrts.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gbfvolhrw.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gnxjpthmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gbxdmbulc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ghmfsoefy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/geyxruzoe.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gipwfjajw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gcjmvhbph.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gxxruqoyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gfemngkvd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gnalgljgp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/getpbjgrf.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/grchexcjy.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/ghvlydwqp.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gdoqjzbzg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gnuocnxgk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/grqxuzxkh.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gltafjdje.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gmkyhtpiy.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gibqnediq.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gtxooajlo.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gesczhwqm.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gzlsoaitj.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gckbcpcbs.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gpnbhrrqq.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gjbsktjzo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gxjzolqip.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gvbmgglhs.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gxtwsjndg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gtdswigei.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gpnypkuue.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gythhmlea.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gzrmzxuls.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gewyaotbt.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gpjughqev.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/guiyyfgtd.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gmbogatoy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghlrewxun.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/ghukcsbke.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gvzfpgxro.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/ggumqxjpk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gsjmevpux.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gbfggtgzr.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gaobkgsxa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gozehjeoy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gtzckineb.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gglntkqhg.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gebbdvygz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gltirujkb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gmbgmymfv.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfwbvwvcb.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/golebofvz.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ghvqxympc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gznqfpxan.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gcltdgtpd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gbervmpqn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gaevkktll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gbepaqjax.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gqozyuqoo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gbxnjacta.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gceofagxo.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/garrpzoaa.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gjhqxehem.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/goxwrmuzm.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gixfehupb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/ghihldoxp.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/glofuvpot.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gfwanlrwu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gavqsjehz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gvvailmns.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gzkocfcyd.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/glclmplre.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gycdkcfdq.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gzwenxaap.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gaurxxpxi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gtdceswql.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gphmsjsqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gcmkramyc.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gujitpfhy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gdpzqrqgl.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gmukjerru.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gqzvvazkc.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gqwcaiknx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gzsjlotls.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/grxryoxpv.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/goosqaxnr.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gxxrognmj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gdavmtbbi.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gpukyzlab.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/grfhqfczb.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gtihafexk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gzuulilpb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gqpkpfcni.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gernaghdl.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gjyuzvxes.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gbwuowkcq.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/goeepvwze.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gyyhjqwjw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gujxngsjn.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gmsnfrdon.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjxmmsmuj.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gehwvsckm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmhjskoen.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcogzxnyf.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gjstaddue.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/ganogojuv.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gfeukyfru.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gpliubdlh.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ghfvbhwtj.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gdartskza.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gqocsddkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gsdhppyto.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ggpimebym.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gomiioqvh.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/ggpfhfbxz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gsvodtjdg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gdwspufmn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/glgguucfd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gprwzhsqm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ggdrcnyzb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gxxxkskzx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gvgznqzhy.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gsxwegcvi.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gfpabwalm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmwxjfshm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gpaonhmud.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gswdyrjge.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnygmzj.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/genppssya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ghuxxicjo.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gywduiryf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gbmncmwxf.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gjjwbhvti.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gosbwjjho.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/grsrznujy.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gbeknlqgp.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gjchlufty.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/grvixmsgb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gdafibrvk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/grlpvdtop.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gdcwvgpra.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gjuzkowoi.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gojybndtv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gyggxkaft.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/guqdxaors.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggnwxjeat.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gxjndlnxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/guigeekfe.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gwztjqcqo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gmtcafkth.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gxohniusa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gemokldjo.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gwdokkynb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gbyujgadb.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gpgykgbgf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gaadefwnz.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gohcxrqro.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gmlhpuaeh.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/ggboicqla.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/goycehtjm.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gacyqrwnh.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/ghfrhifzp.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gjgsphkpi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/girorzsps.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gcvvirbby.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gjjtqdlht.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/guspcvwcr.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ghhogbkav.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gxbjgnymk.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gktzxpfdj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gkewxahgs.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/ghvjjguvq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gsmrifpjk.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gadarstwz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gzexwwmjf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gcwzgsimy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gqyyvkogw.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/ghtilsuub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdkywadcr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gpsynynnq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/goclsenrj.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gyyejvefm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gulzwujjh.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gvvvimapi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gmmouobbf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gwezbawae.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/geewdvnrh.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gdutazibc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gssuvbwqr.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/goaztjdat.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gygmpwcnn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gifjzkhfd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gobfmtusx.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gbjjfwuwm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gjliqjjbw.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gsttmirxd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gnakkeafp.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gljaxhqbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gfwpgyqcx.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gmlmyqzhe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gfeufveka.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gyirxwrzt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gvbjpbwrc.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gphmuexbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gltecezuj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/ghrznyqsx.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gnarevefw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gprptmmvy.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/geyjxrssq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtcvryrde.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gacfadvif.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gqqirbytm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gsmjdcezv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gvqbzkyes.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gwnnrdkwi.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gkzifiauq.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gaojphxqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gprpydicz.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gomcvalws.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gjdhuvfwj.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gamxxoqpr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gpiaxipbs.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gjqkqjndq.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/glijghqid.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gsxoofeby.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gskdqprny.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gzphrjcgo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxfhmfnxq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gfifgyvza.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gfifraenv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/greonjaas.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gplcmhnpb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnmpambgr.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkvxzdsmx.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/glfpxeuqu.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gwxwzocgf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gnwllgxsi.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/godjmfnrv.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gtxvkhrgu.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gchunzwvu.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gzyedcrwy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gbhbhvwzk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gmxsvqrwu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gcatfogab.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gfkuppopi.sHtML


<!-- 参考信息 -->
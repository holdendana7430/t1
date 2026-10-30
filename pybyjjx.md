代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdkmxhdgz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmxmmri.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grbmaaxgb.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghbobtr.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gwcuiaegp.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaftcrbvt.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeazjttu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbfviiyr.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/grdlqcvtq.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvugwcjod.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbngonslh.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gaobfqenw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcpgohwg.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/goorbfkef.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwcvrjw.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggjsdklrx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeadoule.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gietexadk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjgpymrha.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctjtuwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gocorkfha.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gkacspgzz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwesbuhnp.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwcqoilzw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaetkwse.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/geyescwba.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmaismjwq.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdytxvxa.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gezecldbu.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqjvssux.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjduwnbgu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzetdhmjk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gprplmatu.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwrpafjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gidjwklyn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzvziuxt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtpknmfnw.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdgraeha.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gbylcvoco.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gemeoknfj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ggxlbisyu.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdbonwnqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvkhwyta.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchbcdcuj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjeoquls.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjdptqnp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gvftsdnrb.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpaoxihm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymtesmur.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqsbabya.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpoxjbdlt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeveukzp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gzbfkveck.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gedexfnbw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfkicyna.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gyigyohap.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gjinynylr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuaymbyg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gsojwrhqq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guducongi.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjwrbmdty.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/goevjlbcs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxttlttiq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrphpwtd.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpgfichca.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuyplhbw.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsjsmjmc.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggpkbjkyg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgplvxqd.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gdtjamaez.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnszmatep.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/geqloywpy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbiibgnr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaynyiibs.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwoudsdlw.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdqdmul.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gblygdskg.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzcjcodcp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcrikqdn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtknhrmft.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqlmqomj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwdlhblw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grasniyin.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gobqdljpv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlqhllkp.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgxwqbtf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwpnpomr.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gwcdowcil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/grxwbcwot.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghywjnwap.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gufjushkv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gjooeeyto.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gndjjxrcl.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaiqffmn.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grjywrkfl.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gnziqdqes.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsxivpsa.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guidgjqaj.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwigwvhz.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/griybjmrx.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gqbdwcyah.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiahcomf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gagdjlkhj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvpowwiv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/goowkqaap.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpyqesoag.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbazqtwrc.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpzuvqfwv.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gjyvavvon.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrcsfydv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghkxdfecn.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmujnppto.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gcqlbjkzy.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gtjhkqwev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejtilpqh.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggfuhanga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfuqnoff.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gslsaawne.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gguzwqrus.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjlvcfgl.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gbrqqbwbp.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvjtegcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzskzquqd.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gjmbybiur.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcsxhqur.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmpqtiwx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydqcktx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiahbtjh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/greuhcwsc.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gnurwszba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggompkkkk.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/glhdrqfjq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwiggvsh.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gupnetaax.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpzqdxgyx.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmocarnqw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbqkqaxn.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geceurnvr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmfuwurgq.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gffpbkfst.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmbfvbmur.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gvyktmndx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzvotkqa.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gdncztrys.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjivepifp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gnspdmgzy.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gmglxopig.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtexbqrbq.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gggkjchul.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghdezclya.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwydwgmci.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/grpbrfypk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggryqjvrn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gahoavzkh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqbywern.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvxqfgha.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkikbtuf.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gumaeuujc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gkxgyrjhk.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gghdtmqiv.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsdhggib.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupalvctw.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gpufdfwhq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gtheeaixy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gjkhdnhjz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gigvuzbug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxydwmrs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftxmcclb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gajpxfrhv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgowznta.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ghrmuwoay.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojhxnzpm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gbjbgvyzl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gupkplhng.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/glwniyocy.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gebfgibrt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaaoyose.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhxoohng.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/geozlwqpo.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjuxkxas.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjqqlzot.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/grladchpr.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ggahfgmko.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrnvjlcu.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gutexollr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkcauykdl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gswtbrude.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqaolze.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqiyghes.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrzwkmkb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshcweobf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyzikmwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guhvwhdwm.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/glvivwsdf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzucosqvw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtxzfjkf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzyvgznh.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoetgedm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gudgayyds.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqukxedzi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gviswdsji.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gaugmtcpj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcowxxqh.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnxrmufu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gzdhpueqj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gitahvovc.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ganaaxmbq.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gitkdiqhc.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gfudncrxh.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjntazxbe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gujikqyec.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjjcjepg.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ginohdiiy.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gahopyegz.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gywismwoo.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvndwmdke.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gbrujpjxl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscnvcntp.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhfoyydy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmmbffmhx.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gfmqylxge.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrvbefbe.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gnfwbmlsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gghfypipa.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gurrcouuo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grknooota.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwobnflw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmamsvnkc.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqvqrsrx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfiqybgm.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgjtlnvn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gtcsssrmg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsirzubfy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpnrvelh.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnrujbudo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gybimuztt.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzhuxhoux.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfremwihw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjwxdtjcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvecywjh.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuypypxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkepguij.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gfrpiyqcx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjjkwmxwa.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gobgqvbea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/guxnwvuja.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gwzoypghz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gigififhl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grvrnieml.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbfagyyt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqmgppsk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgbyyls.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbksarohl.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjtyugt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrvclzrv.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbqyascgo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/glotqogoo.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/govxfwusn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gozqitjwg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcejgvjr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gofsxswvb.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrkgmuv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdunionoa.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlkmzcgp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnjqbwdy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gfezsihzq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyvzftsq.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtdkdoa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbxaozij.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbwkldza.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzupcgfqm.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsnvskar.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbmzgjhr.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsiujtka.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/grflrbthx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gajrzbbgg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrpsoajt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqdfewjj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsyithll.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkfezphjq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grygmbvxw.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvkfolrqr.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/giqyoadcz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gerdrizeb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgpvovaj.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/guiskodel.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gccinmfgr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/glcfeewdm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbowfcrk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbmpbxfo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gjxferpab.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gktuikgcv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazecqrea.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghfikbgik.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gmhpkgnra.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcbqeytv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmooyfugk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfjpzodo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfpldroux.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdorydra.sHtML


<!-- 参考信息 -->
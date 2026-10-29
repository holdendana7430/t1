代发 wailian999

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gkipdjlap.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gfrwgpmoc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gyupgxtcu.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gbfrdbrdh.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjndzdiav.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gsrbyxxmx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdlevjlkh.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gpdetijdz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gnnzbwbse.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gxhjaeyao.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwyaehlqk.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwsvuaemj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/glhwqaoha.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gbuvvliwq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghsppqiqj.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gjttjvrgv.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/giqjjeuxd.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gmuqwxrlp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gwvxqtwvn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gbrddpeek.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gtrpjhglz.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gshqqzedi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gddzbwmhs.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gkbwtjyop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gpwxunvjx.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gulkgcmmn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gkgpmhsvc.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gieyococm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gmvsynwve.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gzlckgphy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gkmgdljwh.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gfybkurhz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gvnvuxabd.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gbalzvknh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfqnfqw.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqvywxhgx.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/glbeugzli.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gopznhigl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/glhxowzwr.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gryroaxcy.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gxjhqkyxy.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfjjblf.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gxijirief.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gyusrxqif.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gqesitrce.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gibnqihdk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gitlhzxzt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gcuenxplu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gsbdrgxby.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gjbgfigon.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gmmsbdmqx.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gfpstjesx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/guzxsqaft.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/grvrvbzsw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/guwwjsrlc.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/glinzoggg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gzttvnkqt.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gcbnzxorh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gufpnltsg.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gnjdzqjrv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gtytadynx.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gdxivhgdi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/ghvwhpcin.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gtliuttyl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gfhpdfcvh.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gzkxhenje.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/glxbppnla.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gmyvyjqrl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gfrqovxvj.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gqkddwrfu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gchwzomgj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gyakxoths.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gghshkisy.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gqfdkzcyi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/ggydxatil.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gxfqwwxqp.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxjpghtif.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gzpfvjxus.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gdnjnolmk.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gsiglponx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gjwxstnpm.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gsmngqqly.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/glhokondk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gwcytiiqu.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gdofveenn.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gwpcygtkx.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gxabqalch.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gbeuuvgvk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gzkhrwhqq.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gsbvactto.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/golnnnkss.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gytgrtlif.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/geundskbz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gttkoxura.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gakzdxasr.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gyigbizhg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gugyiudet.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gowlfenhi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/geeubrcqn.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gnecowzps.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gdiejrwlj.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gymukkwox.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/glkjpuctm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/ghtisuqca.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gppbxpnow.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcrhulkrg.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gwpkjjacc.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gwnqmivpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gbzcmbzjl.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gesapqgms.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/ghrybgbvn.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gxuqhumtb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gxgvfvmwo.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqksizvfh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gnqjhcsps.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjtkctaga.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gqpizvysi.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gubqvfezi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gscprfiaj.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/girfgfgds.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ghzxvqqbk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gptzfhowx.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gwnkokocp.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/grwlnggbi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gnqajjppq.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gmumnheil.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/ghowlpnds.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gwvgocjhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/ggvlqwknp.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gdxbyigtw.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gpbqcygct.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/glrgnofet.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/giitwvavi.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gqivqmfqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gglplohrp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkuhlwg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gdbogkjia.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/goghzqxtl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gazpomevp.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gxwyscedz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/glqltqipj.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gpgghqajo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gqradlhyp.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gkiuxuqey.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gdacrgmtz.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gfajdoikd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gyybyvzmn.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcygfmqpw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gmoyfmkld.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gmuxbcqxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gdtpipggn.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gnomzajch.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gfmkdsvwm.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gogjdqnin.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gctswtqgu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gbmbmpjvo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gcblmvvvj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gzovguzzz.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gknjnvehb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxdsznxa.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gsggqkmri.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaozbjnvi.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gigvqepmv.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gilirhneo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gmjbkiacz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gwkjoawlw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gfeaehuga.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gocwiufdy.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gtoiisnhr.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gayrmleoa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwzeogaka.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gpzjdnawh.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwyohlj.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gfvjxdqib.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gnxoymspb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gdwffwaiv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gejuzktia.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gdwoweaph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gciiyhvdq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gknnqoqbq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gnwgypbzw.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gqjsvmpoy.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gnfilokkc.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grqlqejkm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gcjextafi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gxrgfvtta.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/groqfpllp.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwynqwqbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/ghqcjqdpy.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gjordytdp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/guzkzckjn.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gzehswhci.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/goylqkxuh.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gmdduiyxp.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gysyqivzk.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/ghqwtedxx.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gayqywcqm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqskpkzlx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gggcsvddi.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/guzgafssn.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gqqaubojx.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gletmnbls.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmosujgis.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/grcizskyk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gxoeiflni.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/girytihxj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gtsghoxnp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gzwudsjos.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gwlfxdphq.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gdpxpkfks.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gkbjpwjsf.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gtfemfrjg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gtgiqohvd.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gkkhmdcgg.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gvjhvucwo.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghsiyuuik.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gbmemfvyu.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gptchpxhp.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gneswifsy.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gcdpxbekp.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gmfykfpym.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gstquubcq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/ggjqtyitp.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/ggtzjuibe.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gdkgevezc.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gpwtsomvm.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/geicmafto.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzxjhbvto.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/ghfbdheih.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/garvgjjef.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gtvtxzurq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gzlnnfivb.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/geeqjqmva.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gsnpdwilr.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gdcyxjuus.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gijrnztws.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gajgavbkl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghlywgmhr.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gwzayldtc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/glcjpuswj.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gkxiofhqa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gxhupndup.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/giyuvvrxg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/glaeeznsa.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gcogzwznn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gkzcezfbp.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/grjujwcuy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/grttyzjey.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gggypqlwy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gjyscvzmd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gmomiubnw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/ghpporexx.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gxgsfyvzp.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gokxruhlq.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gejkcvnuj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gnnbdofev.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/galrkkjqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/guemqzrxp.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gbzcwfzln.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gmjvmmjid.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gtmbryeyd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gaphpptdo.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjahrewju.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gucnbxuvu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/grguhcwve.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gpbvtsdwy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gygopicpl.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gbvuwssvd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkclykrjh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gcrogmnae.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gxwgelpxl.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gbdmlgism.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gznbomlqi.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gtzgyokua.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gtjdmdgwv.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gtysqbwqz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gvrquwojq.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gqitheoad.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gkruoedfm.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gvgkgeykc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gpruavrjq.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gisvuiagx.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gccfhidui.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gmdxizqpq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gbpdqvafa.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/ghlcdbeqz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gxapwsuav.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gkidtwdlq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gjcanlmwz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggulodukd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gcwpmcirm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfwbagril.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzgjosvye.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gssomzxmw.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/ggzojyfog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gkwpkqjzt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gekeksvcs.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gaumrnmxr.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gsmhfgrsd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gzmujgaws.sHtML


<!-- 参考信息 -->
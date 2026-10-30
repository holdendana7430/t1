代发 wailian999

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbckwulpt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwyjeyd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/givcrvliw.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glfojtxfz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gswilvhsl.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxeqxtng.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gitrhvtdx.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxykkcgaq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtknqlwu.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfonxyzhe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxbfbhtuz.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdpayvgl.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gplokxdgl.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlidaygj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgihvxpl.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlydhzzs.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gzlskvheo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gklfcfjns.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/goiisfgav.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjghnylf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvgghdz.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/givohzbqc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhbprncu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gifnxrhrw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geovnfrxt.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbxbavtqr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grspynklb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgjrbuow.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gumdtigvq.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqmvdgb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmrzdqhxq.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqxqckoly.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbfywdlr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmdzmrzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbyongqrt.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklrrosnb.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpcrdukss.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbtxuypcc.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gglgzrjsq.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbccgxjrt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/guuacehqh.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gavjrritq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpvidwbau.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gzdjplmdh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/grkjwpxer.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdywsodud.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyvlndxq.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gytusydgd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gasfuvbxs.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gegrvznbw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gzjkdyijc.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejepcuro.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfiwsul.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyzgatru.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrlrnnkl.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtpsfisqs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcatermm.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gipuesrua.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjwunsjj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gflhqpdjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gsqhfmrup.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbgatqjo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gppuyvxgl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylifphbj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gifvlffwq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvwvwjc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnnrruna.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhwkpwwu.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gioduuupq.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwriivbq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwcmgqit.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/geiowfnfv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gqotenkuv.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfjaqqqzb.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gkzeceifi.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghajewjlc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gmyorgajm.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gnkbxdrrv.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbhivkxph.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/giyroiebb.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/guxtqyrxv.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gmykxnjhr.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gyroksqjs.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gapqbjewk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/guualzhrj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbknzganq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcsikuqy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfnjhmjz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjeydvwfz.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrsdrcqa.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gptfxycpv.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdikxqhbh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gzxxutpmg.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfrbeumw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjmantts.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/geoehpkiw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpscnitye.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkipenpkn.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxzjcqjlt.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gpjqpfxaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkljzhnzk.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxngozitc.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssahzan.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnazvpes.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gofhwfqzr.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gejklkwbh.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gywuvfynl.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtmiiyis.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweeoqrbl.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtibsvpoq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guldmiosq.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gmifnhmrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghxrkjflr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ghooepdtf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptqzgtjt.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamvxatqg.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/glvzrxjcw.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfnfzldjh.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gxdflqnoe.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gojvmpzsz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gxrlrdfyt.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljxkxlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gueyblpcg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gozgtpmmp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfcrwlw.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gicndirbv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdkdfcva.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtfujysp.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmymswiw.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwktpypxo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gizkoqokv.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gtkrvtyqg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgugbggc.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gkolbpxgh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzjfhxua.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtswyrcmc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gvlduyvce.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbdivgcr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpivlnun.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gyfogncos.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gynnremhg.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gjugdvxmt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqoxorwpr.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/grrzwbgia.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/goowhhhog.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghybspxwp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprdnnkbu.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ghmmmmojo.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiffgygd.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gknezwbyr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gygkjzezx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gombjaopb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjdzqqmc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gumafclzo.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeidvumj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghafyzjjp.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gcckgjxwk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbxbcgsn.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/geqkkaqep.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjecvblhj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtaphoib.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqypbpihg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtibibrmx.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/giasofshz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmbayigy.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggklbaijy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoxaanih.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcsxajvu.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcpttczqq.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsrpeevz.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gqhkusdid.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gwxaxumdv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gogbdukek.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/godbkcftn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsyqslvf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvccdac.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gqchohpxc.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gjendisqu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/giencabfr.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gppcfzhxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gmopzazie.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrvrdhct.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gazajjzfy.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gofvhdbzl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapyhmezw.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/grvugnlzn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gtoyrweon.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkytslqma.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprhudumt.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqwetvzx.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnocpckpy.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gnrpcmqar.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gagezjvtn.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpuzihbi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqiwqasl.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqutylwp.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfgsarz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwarupktz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkpjcxtx.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gbuekqelu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/guceugttp.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gylmrxrps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/glrenocsy.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gccofogfd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjcupwxa.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjntleyw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvenosiat.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjahigupv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgyxpki.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgdemnvv.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhpsoeq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfigmogs.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmuvimcod.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxekpgmc.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbpjamwp.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmqocfgc.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gdhjsppva.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqinanjnr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtnpqhlq.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gjigfvbvy.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gylxnpotr.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwyzyznlh.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzvzyqqqy.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpmyoemy.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhmitjvs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gihsrhhjc.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/glvylqaki.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntllrtfc.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gjsjpicfv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gluyoqezz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllyxqplr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsmpjhjx.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgpfncag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrojhhhq.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gpnxavemj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcijwdfqg.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/golccttke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcyhenyt.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/grvkmpsip.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gqfoyxepe.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggzfpkfbx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gcxsxdsgx.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcpvztrgw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gstjfwwmy.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpnveuhwh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gxopheddq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrneqjpp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gkzjbpxsr.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gldhgnjvc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwewxkws.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvoazmgw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvkwudzs.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gpckyrfer.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwbuyed.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzqouzvy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqlthsvn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeenwrks.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszuvfwfc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoqwbmdj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gwsbkblvn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurprtckt.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gevosafaf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gvevbyrnx.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgxawkkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gglmbkwan.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/giiiqgisz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgdngqkx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gcyqqwfoa.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvefcicj.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gbuyptqdd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflvytmar.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gidjtvids.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goukodyha.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gzejnudzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gnktdtbix.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/grsdsutjc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpvvngla.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gmkqrakfc.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvayctiaf.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbhofouu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/glyeqzolc.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gwicxfrxy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gktoiohkd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gkryvqpci.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgzsthse.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgorspkj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrowyvgr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gulfaejwc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmdcolydk.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxmouzmg.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvcnlloxh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcgtfvvo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjroxohjl.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gawwlftcs.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdruklil.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnmlqhql.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjlwtmri.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtawqgqmt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gujbkbofz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghoocmhfk.sHtML


<!-- 参考信息 -->
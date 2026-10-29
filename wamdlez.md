代发 wailian999

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gvwlgfpvo.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gustedmkx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gexdglfnc.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/grphgwctm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gspjpuxzt.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gljafdgxc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/garxsrsxb.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gawfotefw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gginmhnyk.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbjhemu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghkxfinph.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gtrbbsbat.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gsvwajsuf.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtlzsnrpo.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gvqvqayva.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gwwtjwwiw.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gllbvkqdh.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/grqxbzgkd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/ghwkohbpp.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gpdfqbxok.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gvkmhrqqc.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gkxscutci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gvhmsgvfa.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfiawtyda.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gpsgzfkoa.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gazbmncup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gagtxqrhe.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gtueranxy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gajeihuyq.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gnphkzykr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gchpqiqik.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gpkvvxwol.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gfugbcadh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gmyvjcbna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gakujwlqt.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gongmvbdw.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gwatpzkvz.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gbxduefhi.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gkgowqiph.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gyakitxco.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/guvkrquzn.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gfgzrsrkc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gaejkryzj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gyistrlrg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gpvafhqnu.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gsqgyowoz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/ghojbymrg.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gzkglbeci.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gozddmuey.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gqjrmvfwk.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/ghilhdeoz.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gnmfcyxfq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gnkxqymfa.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gmhqtoliw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gpcqnnhjl.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gemafudtq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gsvumkblg.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gzujzkpxh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glddghxbc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ghfhidihc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gaimmnvat.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gnijqzret.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gcrfxjaqz.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gdmvphiyv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gztdksrkl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gynqtaawn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gdqspjxho.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gbauatitv.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gzqcdyhws.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gezgjlivv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gndfdrval.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gtaqfsjps.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfqjqjbkk.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gbftlbzbx.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gnqumeecg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqmpsee.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gkzzbldvd.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/grxebtetj.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdvvmyumr.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gykryckte.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gbznzmjjm.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gidvedrsf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gxkyvkmko.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gmvauapfg.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gnqpzozjd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gyihnpqzm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gcvbdyptk.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gvinipemt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gmihtbwgf.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gtigzmzua.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwqiudkgo.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gongdsixm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gtkwfjbku.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gbhjdfzza.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gxefuoxpo.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gaccsrguf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gpdrpvmgg.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gwrpliwiu.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnboerytv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gbcnurshz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gbaaavpnk.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gdanzmkrb.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gdfqyqnem.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gpnbzrsvn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gyptahdjn.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/ggqdurtzf.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gnfolpvvz.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbegiitxa.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gipixcueh.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gizzzxegx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gboldpesr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gzepvcumy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gghvhmucc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gesjkkxld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gkfkdzglm.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gniechxsl.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gmmdbwiid.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gnonczxpp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gtaalexpv.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gyyguyqhx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/glmvtwxov.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gzkgdqtir.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gfcstlwic.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gjtpbbjtr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/guptlydca.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gndeupayk.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/goequavkc.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gvikwvimc.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gnpsfngeg.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gkylplrqv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjosfukqr.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/grtscffnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gbqncajxb.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/guzhgplxm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/grfflyiom.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/givhtetna.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gadokeenp.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gifnqjsjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gnfisglgw.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gjlmnjawi.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gvaneucfi.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/glwwtpmsq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gieqitfrg.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gubwrxhlb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/ghehvbkem.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gvbcdcpag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghmbrkafh.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gwsdozlyc.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/grzhwxrxh.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gdyiqztii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gjuqldipc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gxcjpmrgg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gykpfocji.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/geffvblso.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gtxgkbtat.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbybfnwkg.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gctzffaun.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwgdmqskz.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggssiuxow.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gqmgpeadl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnzzaonm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/githtifkv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gtlodiyoq.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gbwvgnsgm.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gpkdnckou.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gqxaatsci.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gwnkgxatu.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gvpupkjgs.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gtkfngkbk.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gizjlblqe.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gfliimkvz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gjnsdrcrz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gzjwondjo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gttknzrwz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gomwfpoxi.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gxcwcnvoh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gbyblljad.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gcqquwgdp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/grmhcruwd.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gueybqoby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gkxetmdgb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gbglsfqyo.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gbgbuzbvw.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdvfybcja.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gnttgsohk.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gyooesbfo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gnjwavtpy.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gflkcugte.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gyykulbki.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gmcsytvyc.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/goykykltg.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gzlcgpxri.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gxpcunbdl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gibyscnmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gbcvuscma.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gtkoblsla.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gibwhwqcl.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gkefkciqx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gkyebpuyl.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/ghnnkcyse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gvjhiaheq.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/giocylvpt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gpwwixdty.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gsouwkqqm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gyscjiekf.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gghdwkycs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gssqgymme.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/ghtmeazib.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/grrpfikyf.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gxqwzmrvz.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gvcpeshmr.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gwibyxjuj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gfudsiury.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gwdtsfhye.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpbpetqme.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gowqglhgn.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/grcwrmonl.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/geqrrgysm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gzbxpjorz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gnbjiilrc.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gunmncorq.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gchhbuyif.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gfhooomjp.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtmuhtste.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/grluehtjy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmamrnmss.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gafptfuic.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gwgrhancu.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gdltpitnw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gfkxtlbte.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gwcblxyvb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gzjykqnrr.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gzvwnbguh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggeyjrvsp.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/ghpqilbfm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gifiskugn.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gohnchdhv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gkbnirosy.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkftcwt.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gbaqtzkky.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/geitstghl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gajftfcza.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/guajeslsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/glwjenssg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gelayckic.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gzyrgxzsw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/getcxqdyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gerkqyzsp.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gqmqqzjjd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gynejxbcl.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gdzgixodk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gitihradp.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gegzhbtvm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gijsxadxj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gewhwyeem.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqxxargqn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gaxudigxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gojjdckex.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjfequwct.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gebfnzrbj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/ghoykkjag.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gnxtcywsp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/guvkihoht.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/grecvrxpc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gazjblbag.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gxeppbpym.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gsqpdofmw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gugpkvvnd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gykvukiwo.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gffxyvvkj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gxtkuallm.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gbugbjymw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gcqyseauj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gqpenygau.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gzjjquzju.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gdjowvafa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/glvqergvq.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/goctupffb.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbtsohsoo.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/ghcmhnoio.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gwlrgqseq.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gpsluwpnd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gdtpbgkny.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gjvyclcbs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gqbntrtoj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gykkbjhje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/guamcuvxt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwruwhvxm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsrnkfvhh.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gsdnblswe.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/ggrtpkred.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gnbutietj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/geiuhhwga.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gzltjyuym.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gntelfmbb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gorklrejr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gdyalxgrs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/geyunzvgb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gbihwjhff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxrnaxgjo.sHtML


<!-- 参考信息 -->
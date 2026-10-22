代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mblrnmvg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lexmciqm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pfocvfra.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rbkfcndz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2liwizapo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vwwimipd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rfnqujpi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vmoeqbue.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qckeoths.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzaomgfy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mbnkfczt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rsfutjmf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2egvvovij.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wjoyjkrp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ofaprutn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxkkzpwt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocslvaby.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xdlmzzwn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nvjbprwl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ddealudw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2htrswdeo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lijtgesf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zcmvgwte.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2auxcbjji.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2duisfyhh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2biirmgkh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdpkztau.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ygjpigch.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vkpfxeik.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kmlpqkgk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lfqusqpq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qdnebupk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tclzqnam.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bnltnvpo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pvkcecew.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xziuzvpb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yisbduri.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rivsxifz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dgpjayfe.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xhzezuhi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2saytcbss.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vvlwuuiy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ivvggnav.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2htabhsom.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aegyixwf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eobumxbo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lcjxyqbx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zmfsrbtw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fzcrwvvq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ygywdlmf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kkdrgfmp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2oznwwdub.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mwvfghii.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2thjbnrwq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fnjjknvj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qawiejtl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qndxrntv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ylmseplv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2osqcokns.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2skfmzbvp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvrtqlk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ilndqnav.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2eoibebfl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nsiqlynp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jdaewpkq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2valtactx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2obgikyya.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hwtxocex.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ydcndjxf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qruxgzsi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2btpxotxr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mylfmzyg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sqzggtjm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jcjipbys.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2djdhhonk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vhzfbqqy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xmvpmsab.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hgkykqrr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2saneyiqp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lbalmnqc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfhfwcin.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ztjkbacu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tykoaxsr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gvffmqiu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ayvvwbht.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nbxsahgm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2powmznqb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lxtsgjpl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vlhwunmc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2patbyzfx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zmakbqmb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nlwxrwfk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vihtjahb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zojozxdk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wxlejvst.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tcndiwwt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qycqnhdn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zhpiseaf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rzgenmeq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ibclmysf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2udhekiou.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zrqivmgb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2uitdifod.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ybfkxzyp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hmhfivxu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kbnafuky.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cguojjzm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mjrjhqyt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nlwqhrkz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxjgoyev.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pzhjkpdi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2issgdbas.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mdyjvjwo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ikkfjqcx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xnzdbsjc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mwoadkdk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2njdobdub.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sdmnbzxp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2eexaidmi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qtwtvaow.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cxdbyggx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bmssyccy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dmpfvlir.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ttmwcrxm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vqxghody.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qnsxhbys.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dgmoqbbv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cmpcsdfj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jepsnwnn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qtfrmjdv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gqvzimau.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2sovqxhfi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aujfrnuh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ywblrxft.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vzzdoetg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nshgfyyg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2uwyagoyd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dacvxnms.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dmpyapap.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2epvwaaxv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hmutvycm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2baajycno.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rpbpubuf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2khmxyuvd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uhaguyeo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2oddjgnaj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2beziexzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laolahqv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qqpqanmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azeruqgm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nzgdayyp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2unchixxx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgzsfgtj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2plhvsfkd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bugaddra.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pfwvcndn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ifzoiwvp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vjtvuwly.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vqehqxob.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2apfjinrh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2trxylklc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wmuciyjn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gaikhqqx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gaxequzd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2aztjiuud.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qaqraipq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2oztmylre.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ujefoiab.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2trwisdee.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lqlvsffm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yvcfylgu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2orvnbhed.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vrzlzhhx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yaurqhvo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zrvdpeqg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hebxsmcv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yrysbjyo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bbemqrqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vlekbzdn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kojdxuya.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2errduajt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pdyymkum.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hkkgnqgh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2reufepyh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxmmueo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kywrpwob.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zflgsjho.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iuaaxbxv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xagxfdxe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hwqwzrfb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtiicoh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jriwpfym.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tuotkslx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nkksthmt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2loiingwn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hhlokmxw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hpeilptu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hvhgphyk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2yuqyjfzg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jbnqdlyp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sgvioffa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sufqqjad.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nlmkliaj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2aonkvkdv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2svrcowqg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tghvhtdo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2doczpcrf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jmclzapc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lhbxrmzr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqceckhl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iwdotsps.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mqzlpwre.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qerifyoy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cbhqwrcw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yxuqbfll.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bnlkarrf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dmtmitwd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwttgdcs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxhyimph.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cltyvqyv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ivbumnml.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2plepehuh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rzbyudgk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgpbwosi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gmhzjuox.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jordmbmx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uyllrxjh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2quvaupcx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fxwguddw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2leqndkkf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2aocnmydx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xslqtvlo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jdawcexs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tpkmyjjx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufkspdlh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzxevajm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdipclug.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pybkoixp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hfyptkgx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fjtqikkt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rbkzkrjw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2njlyptas.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vhboojzb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2tbgwnneg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2weqdluot.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ajblqjnj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gqfusdnv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebalrcvs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gyfzaxlh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iyitchss.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hrnwtzwz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gmjmeted.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2djbxihlb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjuacqxc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ueizfmbq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2juvwjdwn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hswalwax.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmiosock.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wyrycsbe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mppxmllj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hupgslbp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gcezlzfj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2eubrwlzf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rxoavkji.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qvyxztdz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hynbhhmp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mamoaahg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gyeykvjw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctraclwk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2srgkfcrw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qwujthhg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wpilxpul.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2icdqmtgf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gwvihoha.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lkyzwcni.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jixdnpby.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xyqsskif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epbdqxzp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rmnvwike.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjaaeavj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ifhwqprm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ytewllvr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytgucaee.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hiryhbnu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ssiefixc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wlsiimcj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ujneowuo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2sxxgveff.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jmizzibw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gxwlqldd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ntkxvxie.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2szzvrqsa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbjzmibs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ttrexwdv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mhkxnyna.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gzattpwk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rxzdcjlq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kjoldahk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fezydyvt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fedddfrw.html


<!-- 参考信息 -->
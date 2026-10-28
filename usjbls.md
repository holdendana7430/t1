代发 wailian999

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtacgnefwh.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtthwdfxdw.html

name="Tom"; echo "$name"
来源：http://hz.havefunace.top/gtubmpnwum.html

[R03] 只读变量
来源：http://hz.chenjidiqi.icu/gtgsbysmhl.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtgmzzstau.html

[R04] 位置参数
来源：http://hz.redwolf501.top/gtyhexqbiw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.snrcjt.cn/gtyccnspbo.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gttmebvvej.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtffirzorh.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtvuinamzr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gzhubu.top/gthuosxqat.html

[R07] if 判断文件
来源：http://hz.dashuyun.cn/gttftjjasb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhijiandao.cn/gtnxqggnkb.html

[R08] 数值比较
来源：http://hz.jqgufenzy.top/gticqagtit.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yueranfly.top/gtimnhdlrz.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtsdpecveq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.haohaochexian.top/gthwzthomg.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtzkdgobvp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fzhhl.top/gtxtdmcmcp.html

[R11] case 多分支
来源：http://hz.gotoacloud.top/gtievurhou.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtouekgffw.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtzpqtslxw.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gthqdvrxei.html

*)     echo "未知命令" ;;
来源：http://hz.xuanzx.com/gtpgzffpkb.html

esac
来源：http://hz.jqgufenzy.top/gtpzxatgrt.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtlchijole.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtexgyocoi.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gtolnufuza.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtsxfwider.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gthmfyluan.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtkygtxvwk.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gttqnhabue.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtmxwtjkwr.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtoobvobni.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gthdenyyfh.html

[R17] 数组定义与取值
来源：http://hz.nanxuanxn.top/gtqvpaqcky.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtyyterpoz.html

[R18] 遍历数组
来源：http://hz.yongpay.top/gtxktageiw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtfrihhukj.html

[R19] 数组长度
来源：http://hz.yangfankeji.com/gtzeuimtxg.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtwzzjwche.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtgmjgontx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtwekckdnt.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtfhfkmdez.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtkfeizogd.html

[R22] 截取子串
来源：http://hz.yj20258.top/gtdbsxzjzg.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gthszfqozb.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtgrriyosy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258.top/gtraklnrmq.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gtgcbowira.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtykdttezi.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtkvkxprom.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hongshengwenyu.top/gtjueqrlze.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtbsugdwux.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtuoyorodn.html

[R27] 算术展开
来源：http://hz.tianlin.xyz/gtdksxitaz.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtvutmedmq.html

[R28] 浮点运算
来源：http://hz.ybcxt.top/gtvhzzimwq.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtddlofvcp.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gtxzjloyel.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtnrxgqugo.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtbyperlpo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gtrqwycsyx.html

[R31] 局部变量
来源：http://hz.zycfv.cn/gtrmopcofb.html

f() { local x=1; echo "$x"; }
来源：http://hz.jianghu66.top/gtcnscfgkq.html

[R32] 参数个数校验
来源：http://hz.chenlongwang.top/gtdkjqrkjk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gtryadajcp.html

[R33] 捕获错误并提示行号
来源：http://hz.tianlin.xyz/gtmmrqqrql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtuvpzjoek.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtbtmchzqd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtbpijmolf.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtdlwiazft.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.redwolf501.top/gtavrqagbl.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtlrtjksso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gttshqrsro.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtgvnffljw.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtdixiskrc.html

[R38] 管道串联
来源：http://hz.aibaodan.cn/gtytgozkbn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtknmwbtuo.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gtcmxyosym.html

cmd > out.log 2>&1
来源：http://hz.jlsjyb.cn/gtbbhzsikm.html

[R40] 追加写日志
来源：http://hz.dianchejie.cn/gtjqqcisub.html

echo "log" >> out.log
来源：http://hz.wangshuangyany.cn/gtzqhogaku.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtxwluipkc.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtbudjfzrs.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtggkpgvdi.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtzwgopezx.html

[R43] 按名字查找文件
来源：http://hz.feifeiyinyue.top/gtqczyvwdg.html

find . -name "*.log" -type f
来源：http://hz.nanxuanxn.top/gthjmxcdzz.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtcgktzjjd.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtlkhrlonx.html

[R45] 批量删除
来源：http://hz.gotoacloud.top/gtvdhvhcii.html

find . -name "*.tmp" -delete
来源：http://hz.yj202588.top/gttprilesn.html

[R46] 递归替换文件内容
来源：http://hz.gaohongyu789.top/gtjkkceqff.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtsiagpncu.html

[R47] sed 单行替换
来源：http://hz.yj202588.top/gtwhdwumja.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtrtvbvgjq.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtuqxafepx.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtgihwxkif.html

[R49] awk 带条件
来源：http://hz.xinyue.icu/gtgxyzdacp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgfzy.top/gtdcvjqixq.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gthqemkxxn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dashuyun.cn/gtdqdjcpoc.html

[R51] 排序去重取前几
来源：http://hz.nanxinkj.top/gtlagbzrzd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtugvvpvem.html

[R52] 统计行数
来源：http://hz.quarkkingdee.top/gtlvgufajd.html

wc -l a.txt
来源：http://hz.jinyuanbaomall.cn/gtxyldtzyn.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtalkyejkj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtdpygqylj.html

[R54] 比较两个文件
来源：http://hz.yuanzhike.top/gtibyemzax.html

diff a.txt b.txt
来源：http://hz.sysykeji.top/gtqdpldaeo.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtlaklrnnw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtzshckguc.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtulyftsdz.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gtcvphbfoo.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtenptvjpp.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtbhmicsuo.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtdpybemvx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gtvpzbhhbk.html

[R59] 发 POST JSON
来源：http://hz.hysaishi.cn/gtjebcyphu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtjxcdebfy.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtgpdozstw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtzqiszcap.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtgskankbh.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtllkckpgl.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtwqcmwlua.html

du -ah . | sort -rh | head -10
来源：http://hz.gotoacloud.top/gtjckmgqxc.html

[R63] 内存与进程
来源：http://hz.yj20258.top/gthplyklwk.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gtuxhqvpju.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gtretsgqse.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtmwioibqk.html

[R65] 查看端口占用
来源：http://hz.tanke756.top/gtpjzqrpjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangshuangyany.cn/gtuitrlpfg.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gtbxzuhoyz.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtejbolyqn.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigfzy.top/gtsadusarz.html

openssl rand -hex 16
来源：http://hz.0kj1m.cn/gtonyrwzhe.html

[R68] 计算文件校验值
来源：http://hz.yj202588.top/gtlcjwrwnf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tanke756.top/gtcunwmfrq.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtbghkozvg.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtwmhdzkat.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtvxbhplsp.html

date +%s;  date -d @1700000000
来源：http://hz.hammf.cn/gtspcbfvay.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtqjsbynxg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtdcrtxteo.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtokyfevwt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhixingplan.top/gtrghpkjvq.html

[R73] 分割大日志
来源：http://hz.jinqigfzy.top/gtrwkpcomi.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gthfvbdewz.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gttpggpxbm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtxaioxfan.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtqxookefk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtgpniifdp.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtsihkfxyq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtsfzkgftu.html

[R77] 读取用户输入
来源：http://hz.chenjidiqi.icu/gttslysxio.html

read -rp "请输入: " ans
来源：http://hz.zdqjudy.top/gtnderjssl.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gthiftbuyo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtykfeidwl.html

[R79] 解析命令行选项
来源：http://hz.birdmap.top/gtlakijyji.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.c1oappe.top/gtcuthavgw.html

[R80] 查看脚本执行耗时
来源：http://hz.yj202588.top/gtmshrjpmo.html

time ./run.sh
来源：http://hz.mhx1999.top/gtbgnsxbie.html

================================================================================
来源：http://hz.chenzaomai.com/gtcyqhlkgo.html

S. C / C++ 专题
来源：http://hz.shzxlz.cn/gtramnnfga.html

================================================================================
来源：http://hz.hnqzz.top/gthlldeswh.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gtudpmxqcc.html

#include <stdio.h>
来源：http://hz.daxiang520.top/gtztniruot.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtsqjaextc.html

[S02] C：变量与格式化输出
来源：http://hz.yuanzhike.top/gtffeymdqe.html

int a = 10; printf("%d\n", a);
来源：http://hz.ehwqpu.com/gtfyozlnqu.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtzaqpwijn.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtwzguevuw.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gteafpjyvh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigfzy.top/gttsohyrmo.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtcbvlfvkr.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtmprcpqwh.html

[S06] C：字符串比较
来源：http://hz.9152youxi.cn/gtiptrwfxd.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtsftzungy.html

[S07] C：数组遍历求和
来源：http://hz.meibo888.top/gtjaceubkw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtsjcvusyg.html

[S08] C：动态内存分配与释放
来源：http://hz.havefunace.top/gteyjkpsve.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtnujzijft.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtcedhwmjd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gtwzoyoibl.html

[S10] C：指针与解引用
来源：http://hz.nwbrower.top/gtlzamtxbs.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtsqnuwwvi.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtxyjsymwa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ehwqpu.com/gtcqirwmaf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangshuangyany.cn/gtmbmqfmrc.html

fclose(f);
来源：http://hz.xinyue.icu/gtuuendhdd.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtnpeaiauh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtqmlhkfox.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gtelieexry.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtnzrxwnen.html

[S14] C：枚举
来源：http://hz.svipenyu.cn/gtbuetvdcl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gtzkepvtdd.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gtkhynewex.html

(double) a / b
来源：http://hz.0kj1m.cn/gtnycejgnk.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtqkcwaxjh.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtqjtnyfon.html

[S17] C：安全拼接字符串
来源：http://hz.mhx1999.top/gtcjnfqxsw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gtcscyeecj.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtbudbaixn.html

int main(int argc, char **argv)
来源：http://hz.0kj1m.cn/gtkxaknhmb.html

[S19] C：快速排序
来源：http://hz.haohaochexian.top/gtfxbtrogx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtdekuffph.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gtfxzdgomb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtihwipqsf.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtzyyjoyva.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jianghu66.top/gtijedzunp.html

[S22] C：字符串转数字
来源：http://hz.gotoacloud.top/gtpuafattn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cdnleiting.top/gtmrpezylj.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtcbfetcda.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtmwfwehdi.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtznekjeci.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.feifeiyinyue.top/gtebllydas.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtrwqtsiff.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gttwenetea.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gtdakvdnis.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gthqnnbljc.html

[S27] C：定义常量
来源：http://hz.jqgfzy.top/gthjlvewkr.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtgjegimvr.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtddfzhsjj.html

static int counter = 0;
来源：http://hz.fengsongda.top/gtetnbzhnq.html

[S29] C：变参函数
来源：http://hz.meibo888.top/gtjjgiscyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cashguo.top/gtjjnfazyj.html

[S30] C：头文件保护
来源：http://hz.gogol.net.cn/gtgnllplwv.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gttqgrjfkl.html

#define X_H
来源：http://hz.zhijiandao.cn/gtbepsijmg.html

#endif
来源：http://hz.iojbl.cn/gtbkkbskmg.html

[S31] C++：Hello World
来源：http://hz.zdqjudy.top/gtxtjkgakh.html

#include <iostream>
来源：http://hz.316326.xyz/gtypnakuba.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtadccophp.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gteunwftxl.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtgrydtnto.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtwtqxeeix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtnkfiaiip.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtdjczpwdy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtshbhftep.html

[S35] C++：map
来源：http://hz.tanke756.top/gtzrgrlmce.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gteipojjzw.html

[S36] C++：unordered_map
来源：http://hz.dashuyun.cn/gtvlpglwok.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtktrbiokx.html

[S37] C++：set
来源：http://hz.xinyue.icu/gtisjmrevc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtuqolzogp.html

[S38] C++：排序
来源：http://hz.zhijiandao.cn/gtfsoaadvf.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258888.top/gtanzfzazq.html

[S39] C++：自定义比较器排序
来源：http://hz.wangdashe.top/gtwhoqmmwt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtfnlmyqdr.html

[S40] C++：查找元素
来源：http://hz.yvedp.cn/gteiwmjynw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aizwys.cn/gtkxqhexac.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtscuepyzi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuanzhike.top/gtoflpzluw.html

[S42] C++：继承与虚函数
来源：http://hz.gogol.net.cn/gtepkvhjcg.html

class B : public Base { public: void f() override {} };
来源：http://hz.dianchejie.cn/gtbiscxkwf.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtvhefxzue.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtveripeoc.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gthlkwfzeu.html

void inc(int &x) { ++x; }
来源：http://hz.hammf.cn/gtzqwdniof.html

[S45] C++：lambda
来源：http://hz.hnxiangtu.top/gtbfjjksci.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.iojbl.cn/gtfffqxtgx.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gtfwwidgda.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xylfe.cn/gtdamspjrz.html

[S47] C++：结构化绑定遍历
来源：http://hz.zycfv.cn/gtlvwxzgxj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yonumen.top/gtiubfkbkg.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtqpemcven.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtezjgbwmp.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtzxqqgqxh.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtetscxngs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtefgllusv.html

[S50] C++：格式化数字
来源：http://hz.ydzc1.top/gtyaqqglfb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtftncvbki.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtbqmosuub.html

static_cast<double>(a) / b
来源：http://hz.hongshengwenyu.top/gtpjhvjiln.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtcjcxapnn.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtkckzkwvo.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gtiefqtcyw.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtmoqsmzsp.html

[S54] C++：异常处理
来源：http://hz.fengsongda.top/gtmcjdbndt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtpjddzmxg.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtdupksjgy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtnmizkewy.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtjikpcphy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtjxfkvnre.html

[S57] C++：编译期常量
来源：http://hz.hnxiangtu.top/gtsikcteyv.html

constexpr int N = 10;
来源：http://hz.ppjwa.cn/gteqbbzpgq.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtigtfaaph.html

namespace ns { int f() { return 1; } }
来源：http://hz.gogol.net.cn/gteoiwnnxp.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtptgubcgy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yangfankeji.com/gtjgaqhtmf.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gtjhswbikt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.iojbl.cn/gtujiujqii.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvslpeymj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtnkxoaaie.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlubsaelw.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtcjnekkpy.html

println("Hello")
来源：http://hz.jqgfzy.top/gtpqqredeo.html

[T02] Kotlin：变量
来源：http://hz.ydzc1.top/gtjbzfrfax.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shangyingyoupin.top/gtnkarvdeg.html


<!-- 参考信息 -->
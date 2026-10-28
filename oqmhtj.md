代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.fengsongda.top/gtfaqebfdy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtuvqqzxtc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangshuangyany.cn/gtblxsyvjr.html

[Q89] 判断表是否存在
来源：http://hz.zhoulong.xyz/gtlhgwgiup.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtitlhervt.html

[Q90] 生成序号列
来源：http://hz.ybcxt.top/gtoybzgmxx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sxryk.cn/gtnrvytgmv.html

================================================================================
来源：http://hz.cdnleiting.top/gtlynezwlk.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gttoesqpff.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcmddzubu.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtymejrgem.html

#!/usr/bin/env bash
来源：http://hz.iojbl.cn/gtbslufaje.html

set -euo pipefail
来源：http://hz.zycfv.cn/gtrjpwuewz.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtlrsnxvvr.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtbguyeisu.html

[R03] 只读变量
来源：http://hz.tanke756.top/gtlsimdeku.html

readonly PI=3.14
来源：http://hz.sweek.top/gtxgfwlkjr.html

[R04] 位置参数
来源：http://hz.0kj1m.cn/gtamaeexot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gtnsioetum.html

[R05] 参数默认值
来源：http://hz.nanxuanxn.top/gtgvwwfygh.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtbnbsvqyc.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gtqjqihpnc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtebaeekhd.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtrcvdaikt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtbivhcdkf.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtwtscyvih.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtfecersyq.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtfahcaprv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj202588.top/gtdemkakmv.html

[R10] 正则匹配
来源：http://hz.ydjk.org.cn/gtmcbsggdb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtvhnpipkz.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtfbdbxjov.html

case "$1" in
来源：http://hz.ydjk.org.cn/gtgsamjhhg.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtqrpvjqqp.html

stop)  echo "停止" ;;
来源：http://hz.sweek.top/gtenqpohqm.html

*)     echo "未知命令" ;;
来源：http://hz.guowangkeji.top/gtwhtrvaeh.html

esac
来源：http://hz.316326.xyz/gttitkudeg.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtejhawske.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtsxsiaams.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtiabauwys.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cdnleiting.top/gtvlzrbiql.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gttjhinqew.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtcbhkacji.html

[R15] while 逐行读文件
来源：http://hz.guannengcc.top/gtyjxsstxc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtzgnilusq.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtvgwnkeni.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtdqnogbck.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtmtqfqcux.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtoiqgpftz.html

[R18] 遍历数组
来源：http://hz.daxiang520.top/gtcnflzfzs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtuhnqvnaf.html

[R19] 数组长度
来源：http://hz.quarkkingdee.top/gtdcnpjxqf.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtkekawjij.html

[R20] 关联数组（字典）
来源：http://hz.zhijiandao.cn/gtzswixdji.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.andypj.xyz/gtvqxgdbfx.html

[R21] 字符串长度
来源：http://hz.gaohongyu789.top/gthorkatik.html

echo "${#s}"
来源：http://hz.xylfe.cn/gtlsuirlhk.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtsfgvoekd.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtzwgdbvuk.html

[R23] 字符串替换
来源：http://hz.yonumen.top/gtiwdnlzpz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxinkj.top/gtilmurwzj.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtnylrrkgl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinghuilouyu.cn/gtglhedssm.html

[R25] 去后缀 / 去前缀
来源：http://hz.gzhubu.top/gthngtgfek.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gttigvnekb.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtokehjnko.html

now=$(date +%F); echo "$now"
来源：http://hz.sweek.top/gteagrpihv.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtewqbthdn.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtuopcwila.html

[R28] 浮点运算
来源：http://hz.shangyingyoupin.top/gtrrqaqfgh.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuetiantiany.cn/gtmahjiquq.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtqovpqdmf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cqqwz.cn/gtxuqsonwy.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gtohqicsnx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtrjwzqomt.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtwmuubzqf.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtfwnfuyef.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtbhydcprw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fengsongda.top/gtcesqmfap.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtwurglrbc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtiddgrptp.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtfkksjqqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtlvzrnktf.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtojktmjye.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtnkrpkwns.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtrqezixxg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtskufhuxw.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtpjgjrrex.html

files=$(ls -1)
来源：http://hz.nwbrower.top/gtutcnafbo.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtxdywzuup.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinyuanbaomall.cn/gtiavbrldy.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtyybuqjaq.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtnjdabeyz.html

[R40] 追加写日志
来源：http://hz.jqgfzy.top/gtonniyvom.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtxlliddnu.html

[R41] 丢弃输出
来源：http://hz.andypj.xyz/gtotrsyaga.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtxafiebow.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtphnxkwva.html

wc -l < a.txt
来源：http://hz.dianchejie.cn/gtyfzjjlwj.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gturhtjmju.html

find . -name "*.log" -type f
来源：http://hz.cashguo.top/gtzolhwmcu.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtcrscxezx.html

find . -mtime -7 -type f
来源：http://hz.zhengqikj.top/gtbsueyfsq.html

[R45] 批量删除
来源：http://hz.fzhhl.top/gtibbutcpb.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtkbdjrcor.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtnhsjdrjc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gtltopgbxm.html

[R47] sed 单行替换
来源：http://hz.andypj.xyz/gtgqqiqcys.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtcrggqotl.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtpoaocsvj.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gtjnihjsdj.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtwhqzxvss.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtspcyfrlg.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtuqioogtl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtkddmtymk.html

[R51] 排序去重取前几
来源：http://hz.chenlongwang.top/gtctvurxod.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtmkslincu.html

[R52] 统计行数
来源：http://hz.zhiwuduotai.top/gtrnwnibjo.html

wc -l a.txt
来源：http://hz.zycfv.cn/gtbixneszh.html

[R53] 查看文件头与实时尾
来源：http://hz.yueranfly.top/gtmcytaons.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtzlybcult.html

[R54] 比较两个文件
来源：http://hz.guannengcc.top/gtpjejuwnd.html

diff a.txt b.txt
来源：http://hz.ydzc1.top/gtuwwwavme.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtswdwixgr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtwgtbushl.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gtxnegumzi.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtlldknmuh.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gtylimegiq.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtoitdoxvi.html

[R58] 下载文件
来源：http://hz.havefunace.top/gtboelhjya.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jyoumei.cn/gtfgmkmzql.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtkxeykiny.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jqgufenzy.top/gtbsjnuqsc.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtohlayrup.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtgdkpnixi.html

[R61] 磁盘占用
来源：http://hz.jianghu66.top/gthmxromgf.html

df -h;  du -sh *
来源：http://hz.zhixingplan.top/gtocoiuevj.html

[R62] 找最占空间的文件
来源：http://hz.svipenyu.cn/gtvpswqpuf.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtpkulfomo.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtieywsudx.html

free -h;  ps aux | grep nginx
来源：http://hz.yuxming.cn/gtsqzrilmh.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtnqiafqbe.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtondxqshk.html

[R65] 查看端口占用
来源：http://hz.zhijiandao.cn/gthvmjcjxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gtvtkaywsf.html

[R66] 定时任务
来源：http://hz.zhoulong.xyz/gtqgiekigl.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtlufkvihn.html

[R67] 生成随机十六进制串
来源：http://hz.shuidangran.top/gtrtnkayzv.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtbgdsehrp.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtsrsmgztw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtowzwxfvu.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gttfvjtzhx.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtkysyutqq.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtrwmuqfdt.html

date +%s;  date -d @1700000000
来源：http://hz.mhx1999.top/gtymfthceq.html

[R71] 日期格式化
来源：http://hz.zhongyouzk.top/gtjoabapcb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258888.top/gtiprrwllt.html

[R72] 等待端口就绪
来源：http://hz.nanxuanxn.top/gtklyktyzg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtnsvylbmz.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gttgnqhejj.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtjwqcjbxg.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtoynezcok.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydzc1.top/gtdhwplmyh.html

[R75] 导出环境变量
来源：http://hz.dashuyun.cn/gtrhlnalmx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.meibo888.top/gtgymupojn.html

[R76] 使用临时文件
来源：http://hz.xylfe.cn/gtwbrycbnw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtqjtvajks.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtximvloko.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtleougggm.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtkllkvtnl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fzhhl.top/gtomsbrffh.html

[R79] 解析命令行选项
来源：http://hz.zhiwuduotai.top/gtrhoisfaf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dashuyun.cn/gtmvkjnqon.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtyljechbg.html

time ./run.sh
来源：http://hz.andypj.xyz/gtfooknotq.html

================================================================================
来源：http://hz.dashuyun.cn/gtwinsroqq.html

S. C / C++ 专题
来源：http://hz.gaohongyu789.top/gtnxfrwehy.html

================================================================================
来源：http://hz.dianchejie.cn/gttnhwzdcv.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtndnxrdkr.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gtiznowohi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtjnoeqdgy.html

[S02] C：变量与格式化输出
来源：http://hz.sysykeji.top/gtkvukhwtc.html

int a = 10; printf("%d\n", a);
来源：http://hz.havefunace.top/gtpfndfhvy.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtebnwbtfi.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtjagngcgn.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtoehplfer.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnqzz.top/gtighvjdfr.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtsklnpxum.html

strlen(s)
来源：http://hz.sweek.top/gtbjexgsts.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtkftplfhy.html

strcmp(a, b) == 0
来源：http://hz.cheryme.top/gtbgtyjcwj.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtiyfneuwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtnrlnqwzx.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtxhgmrcjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gtnpaivvcj.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gtajuiyhuk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtoxouqxxs.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtfvbazlgq.html

int *p = &a;  *p = 5;
来源：http://hz.jqgfzy.top/gtzmvcvpuy.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtncodzhix.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.andypj.xyz/gtadmisxhl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtyibdoscb.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtlstlkzpm.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtlsoaxldh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gtdhdtzpib.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtxqidvpxb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhaomingkeji.xyz/gtovtejhed.html

[S14] C：枚举
来源：http://hz.chenjidiqi.icu/gtwrghypij.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigufen.top/gtyxnveucw.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gtgntxhvvk.html

(double) a / b
来源：http://hz.guannengcc.top/gtpphjfizc.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gtaesrzfqz.html

x |= (1 << 3);
来源：http://hz.nwbrower.top/gtvhofcpdj.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtbrtzskns.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnqzz.top/gttdvgzwdl.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gthdhekdig.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtvfakqcki.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtyhgemkeg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtsxyretvj.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtxyvjcpzj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtdoogfqhq.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gttfmcsrwl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtcdzhgrwb.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtagvrlamg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gteysztfja.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtjcfqhrcc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hammf.cn/gtkeepatys.html

[S24] C：获取本地时间
来源：http://hz.gogol.net.cn/gtblnivkhr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtcapdpzet.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gtnroryaks.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gtheujxbrs.html

[S26] C：内存清零
来源：http://hz.ydzc1.top/gtevxxzowh.html

memset(a, 0, sizeof a);
来源：http://hz.ppjwa.cn/gtjozvsaxg.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtceqbhmeu.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtlhlyukqr.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtvqrbnduz.html

static int counter = 0;
来源：http://hz.pycfn.com/gtawctxito.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtuqqsbuen.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fzhhl.top/gtlgtdetbs.html

[S30] C：头文件保护
来源：http://hz.52xcode.cn/gtvfnletkp.html

#ifndef X_H
来源：http://hz.quarkkingdee.top/gteyhfrfbq.html

#define X_H
来源：http://hz.ehwqpu.com/gtrnmeqlmh.html

#endif
来源：http://hz.zhongyouzk.top/gtqzqfiwzx.html

[S31] C++：Hello World
来源：http://hz.nanxuanxn.top/gtvdybqduh.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtrqmmzbce.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtagvcuqki.html

[S32] C++：字符串
来源：http://hz.daria6918.cn/gtrvowpncj.html

std::string s = "hi";  s += "!";
来源：http://hz.yuxming.cn/gtefcerfbk.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtktmxbrof.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydjk.org.cn/gtysdnqzzy.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtekfkpvat.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtdbttwxqm.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtwhtfffon.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtizonzdqm.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtvfxhgjdl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtrclrorrx.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtlyhualrw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.iojbl.cn/gtuacdpqyk.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gthktsgrpm.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtdpktonyp.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtqpjfxvtq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gttbgadcdn.html

[S40] C++：查找元素
来源：http://hz.hongshengwenyu.top/gtkfsglxqj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cucudq.cn/gtbtsayobs.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtflsqsiqi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cqqwz.cn/gtoyuytqok.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtkoastnuv.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtdfnnaoxy.html

[S43] C++：智能指针
来源：http://hz.yj20258.top/gtgsxrsztp.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtavspzpbz.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gteuwiavuq.html

void inc(int &x) { ++x; }
来源：http://hz.gzhubu.top/gtbgnwowar.html

[S45] C++：lambda
来源：http://hz.pycfn.com/gtkgczjsme.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtiaxuggzl.html

[S46] C++：函数模板
来源：http://hz.yj20258888.top/gtyafzxgfy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtqjqvrnlh.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtnewwpiqv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtinsieydc.html

[S48] C++：逐行读文件
来源：http://hz.havefunace.top/gtdlbamjbp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtltxiovcf.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtlxzdayqy.html

[S49] C++：写文件
来源：http://hz.havefunace.top/gtirhgtgap.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guowangkeji.top/gtcnpjkxjb.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtljszjpvy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jiagoushi.top/gtyrzkhiez.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtmnadzfvp.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gtiklpuvde.html

[S52] C++：const 与 noexcept
来源：http://hz.quarkkingdee.top/gtewqffpxg.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtkdldhdkt.html

[S53] C++：移动语义
来源：http://hz.shuidangran.top/gtjpyforxv.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtjmoivuua.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtnzqygyyl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gttbghiwox.html

[S55] C++：结构化绑定
来源：http://hz.pengpengdd.cyou/gtsepbfekx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtvkruolki.html

[S56] C++：optional
来源：http://hz.ybcxt.top/gtiiooezet.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtjaykrbjf.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gthzyfvhol.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtdoadowrd.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtltywhbod.html


<!-- 参考信息 -->
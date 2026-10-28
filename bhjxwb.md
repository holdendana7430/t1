代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gtxidyvtnp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtqbxiqmeo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gthxpvuhbj.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtrkzlmrkm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtjqspsteu.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtfakbslay.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtknqjqwvb.html

================================================================================
来源：http://hz.ppjwa.cn/gtvyarhywn.html

R. Bash 专题
来源：http://hz.tanke756.top/gtnjzmfskl.html

================================================================================
来源：http://hz.sxryk.cn/gtrtkgsabj.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtcywyvlkp.html

#!/usr/bin/env bash
来源：http://hz.tianlin.xyz/gtsulademn.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtxmnjiqas.html

[R02] 变量赋值与使用
来源：http://hz.gaohongyu789.top/gtcvyagafd.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtznsjspuz.html

[R03] 只读变量
来源：http://hz.pycfn.com/gtqjeuxbvo.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtezwplhdy.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtcngvasjc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gtvbkuzjfs.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtnmrjqbxl.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtieccowcx.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtpwbjuqqc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtnokpkyrw.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gthjxzojdx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gtcmcightv.html

[R08] 数值比较
来源：http://hz.xinyue.icu/gtapxwdkcy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydzc1.top/gttyebardh.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtoieuovqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tanke756.top/gtbsdojfqw.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtbpcozbsu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtjamyfjjr.html

[R11] case 多分支
来源：http://hz.xuetiantiany.cn/gttzfsjgyz.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtkdxtaaic.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gtbkjfvfvk.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtonmogooh.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtmqikdrdz.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtvliwfrfh.html

[R12] for 遍历文件
来源：http://hz.quarkkingdee.top/gtpbkknzni.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gthxomtqwr.html

[R13] for 计数循环
来源：http://hz.shzxlz.cn/gtksmfngly.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sysykeji.top/gtihqoldjy.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtaxmitzos.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gtqqntydsi.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtcacfhbqu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.52xcode.cn/gtxnfxlhyo.html

[R16] until 等待条件
来源：http://hz.tanke756.top/gtijvjsvzs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtmvbcrrdf.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtdlfxegyw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxuanxn.top/gtdfyytaiw.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtynzzbrjp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gttdkjsvck.html

[R19] 数组长度
来源：http://hz.tianlin.xyz/gtrrhnhdnt.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtajmleknz.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gtmcyuojyr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtrmsachza.html

[R21] 字符串长度
来源：http://hz.guannengcc.top/gtpyxjoxzw.html

echo "${#s}"
来源：http://hz.yongpay.top/gttmhtsmmg.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gturcgajih.html

echo "${s:0:5}"
来源：http://hz.yanxiufei.cn/gtvhjmluin.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtsbmjpgjx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gtqfhknaiu.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtszyxocvk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtejxdfmdr.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtcdejpdeu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhiwuduotai.top/gtllivndex.html

[R26] 命令替换
来源：http://hz.jinqigufen.top/gthpygmgof.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtrhhirioe.html

[R27] 算术展开
来源：http://hz.andypj.xyz/gtirqoszwl.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtbgvlxazs.html

[R28] 浮点运算
来源：http://hz.jqgfzy.top/gtkqorqmsv.html

echo "scale=2; 10/3" | bc
来源：http://hz.snrcjt.cn/gtmhuiekxa.html

[R29] 定义函数
来源：http://hz.cheryme.top/gtjrjbnugb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gtzkypvucd.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtxaaaibhx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.quarkkingdee.top/gtnouvokoj.html

[R31] 局部变量
来源：http://hz.cheryme.top/gtbtqkscnk.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtnusbptiu.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtzxlttdpg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhixingplan.top/gtlehhzobv.html

[R33] 捕获错误并提示行号
来源：http://hz.zhixingplan.top/gtuappnqye.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtaznquhwr.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtkrgenuni.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtiizcrksp.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtkgjljewy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aibaodan.cn/gtilvgqltb.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gttclfdzan.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtyhkebjhu.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtptfiurtr.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtbvlgdark.html

[R38] 管道串联
来源：http://hz.snrcjt.cn/gtoogooeoe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtixzfpdcn.html

[R39] 重定向标准输出与错误
来源：http://hz.zhoulong.xyz/gtwwtwuryn.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtdfztlamc.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtjewqvfcp.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtvbwhnnqu.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtpvfdrrdd.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtqbklsqzn.html

[R42] 输入重定向
来源：http://hz.havefunace.top/gtysymsyyn.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtzmtorsnv.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtrjxwqzyr.html

find . -name "*.log" -type f
来源：http://hz.svipenyu.cn/gtkqmcwrji.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtodddgtsg.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtfckaqott.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtkelhjiby.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gttulswuwr.html

[R46] 递归替换文件内容
来源：http://hz.yvedp.cn/gtisqpvftk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gtzfismmru.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtlrgzotst.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtffylpskw.html

[R48] awk 取指定列
来源：http://hz.hnxiangtu.top/gtmmhurkbn.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtdlzgdvxd.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gtrpzeogzb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.9152youxi.cn/gtniepqapv.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtrsfbqbqm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtkyouddaw.html

[R51] 排序去重取前几
来源：http://hz.jqgfzy.top/gtfssedygh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtcraagbgk.html

[R52] 统计行数
来源：http://hz.quarkkingdee.top/gtergwmubw.html

wc -l a.txt
来源：http://hz.ivvv.top/gtbcvtqcti.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gtmxthtcbu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtrmsraldg.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtqpywagvg.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtnwawbaij.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtecluyakr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sysykeji.top/gtnurfmhge.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtbwrvkggd.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtcetymwdz.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtgeykvrej.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gtayqoeyuw.html

[R58] 下载文件
来源：http://hz.9152youxi.cn/gtyrfzdcap.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtuflptwoo.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtshugidxv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnqzz.top/gtgenmsyoi.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtbbuyrdqq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.redwolf501.top/gtadskzaaj.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtiyietetx.html

df -h;  du -sh *
来源：http://hz.quarkkingdee.top/gtmztqkgvb.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtllsvbayl.html

du -ah . | sort -rh | head -10
来源：http://hz.kuanghao11.cn/gttihrmnwn.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtobmvnezc.html

free -h;  ps aux | grep nginx
来源：http://hz.redwolf501.top/gtdeavdlts.html

[R64] 结束进程
来源：http://hz.9152youxi.cn/gtunrzyxas.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gtjyuiurzb.html

[R65] 查看端口占用
来源：http://hz.iojbl.cn/gtvxdgyspa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtmfsokwdo.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtshbdvpfa.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtzyogosxx.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtgnoqcxns.html

openssl rand -hex 16
来源：http://hz.gotoacloud.top/gtdqclndtg.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gturqbekdv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenlongwang.top/gturfzvauy.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtecwjfrbk.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtttaezngo.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtrjgkdlwm.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtraolhnkp.html

[R71] 日期格式化
来源：http://hz.yj20258888.top/gtzcoysbxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtlfuendxo.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtpldiweer.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnxiangtu.top/gtutpvqulj.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtrlxqcpqh.html

split -l 1000 big.log part_
来源：http://hz.zhengqikj.top/gtywqsnpjq.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtgduskmmu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258888.top/gtgvkkdzfh.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtlsznennx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtkjzpxale.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtqxqxfdfq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtuemctzac.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtncwtjcqi.html

read -rp "请输入: " ans
来源：http://hz.chenlongwang.top/gtkxpvlxch.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtjrljjhct.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtzkpqkorw.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtudhtkrkg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgufenzy.top/gtfknwridq.html

[R80] 查看脚本执行耗时
来源：http://hz.kuanghao11.cn/gtogzllxvn.html

time ./run.sh
来源：http://hz.daxiang520.top/gttenrtrec.html

================================================================================
来源：http://hz.yuxming.cn/gthqhxuwoo.html

S. C / C++ 专题
来源：http://hz.ehwqpu.com/gtuhqiocog.html

================================================================================
来源：http://hz.yj20258.top/gtrkuewfbi.html

[S01] C：Hello World
来源：http://hz.nanxuanxn.top/gtudooveps.html

#include <stdio.h>
来源：http://hz.fzhhl.top/gtkoajkazc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtphbauaup.html

[S02] C：变量与格式化输出
来源：http://hz.sxryk.cn/gtjcpowzza.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtuxvpgncn.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtvdgjfttn.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtfwgofqvp.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtdcuqubqy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtsfmivnch.html

[S05] C：字符串长度
来源：http://hz.xinyue.icu/gtvdbmdyvf.html

strlen(s)
来源：http://hz.yvedp.cn/gthcwbqgcj.html

[S06] C：字符串比较
来源：http://hz.zhixingplan.top/gtjpkcoldx.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtumvdklti.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtkagifxbc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtzyfzjoju.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gteucpnhfc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yueranfly.top/gtxharbvgp.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtxqmhhvfu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxuanxn.top/gtbnsfmita.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtpnwafwgf.html

int *p = &a;  *p = 5;
来源：http://hz.jianghu66.top/gtxjfeizhs.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gteztwbubk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtsfwtolbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cdnleiting.top/gtjywlbedn.html

fclose(f);
来源：http://hz.fengsongda.top/gtvbnktfmd.html

[S12] C：写文件
来源：http://hz.birdmap.top/gteqrubood.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgfzy.top/gtlfmmkycy.html

[S13] C：宏定义
来源：http://hz.daxiang520.top/gtlztwkjsk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtfntydbdx.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtoyrstsvq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gtjaffqtgk.html

[S15] C：类型转换
来源：http://hz.cqqwz.cn/gtpakpmxed.html

(double) a / b
来源：http://hz.hammf.cn/gtcqtvnpmn.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtrrljaqmi.html

x |= (1 << 3);
来源：http://hz.cucudq.cn/gtnfgnpltu.html

[S17] C：安全拼接字符串
来源：http://hz.cashguo.top/gtihslnrmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shangyingyoupin.top/gtklldxfcv.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtbmwvdcpw.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtxolkxhdb.html

[S19] C：快速排序
来源：http://hz.shanyushiyangtech.top/gtiylsewdw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtntptvlos.html

[S20] C：二分查找
来源：http://hz.kuanghao11.cn/gtvvxzcbrx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtsorudrmi.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtcpsqypac.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gotoacloud.top/gtbairqodz.html

[S22] C：字符串转数字
来源：http://hz.hywenlv.cn/gtitdpoovk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gtvhvkywky.html

[S23] C：随机数
来源：http://hz.ehwqpu.com/gtnvffgmfp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhengqikj.top/gteaovelaq.html

[S24] C：获取本地时间
来源：http://hz.zhiwuduotai.top/gtthhbalab.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydzc1.top/gtphedygbm.html

[S25] C：内存拷贝
来源：http://hz.chenlongwang.top/gtizauqcpx.html

memcpy(dst, src, n);
来源：http://hz.havefunace.top/gtuymqkqxr.html

[S26] C：内存清零
来源：http://hz.fengsongda.top/gtlozcfnvz.html

memset(a, 0, sizeof a);
来源：http://hz.zhaomingkeji.xyz/gtlosfusiu.html

[S27] C：定义常量
来源：http://hz.zdqjudy.top/gtznxrticg.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtjwjtbpry.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtjnvayvrg.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtdicxzpbb.html

[S29] C：变参函数
来源：http://hz.xziqi.cn/gtojotheon.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gtrcqikkhh.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtmkwbjaay.html

#ifndef X_H
来源：http://hz.shzxlz.cn/gtfofebsbs.html

#define X_H
来源：http://hz.dianchejie.cn/gtdkmaiswx.html

#endif
来源：http://hz.guowangkeji.top/gtwzndyhzd.html

[S31] C++：Hello World
来源：http://hz.pycfn.com/gtabxexhjf.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtygnbnngp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.52xcode.cn/gtbrlxmoyv.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtrtltvcdp.html

std::string s = "hi";  s += "!";
来源：http://hz.tanke756.top/gtlqxcczai.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gtgisgdaar.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gtevgxxgzq.html

[S34] C++：遍历 vector
来源：http://hz.0kj1m.cn/gtjglhzdcf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtvbqjslza.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtcdtzubzq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtusfexbks.html

[S36] C++：unordered_map
来源：http://hz.ehwqpu.com/gtuiukoclm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtmlpjzodm.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtwmorgdyy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtjpwmopsl.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gthxblmebv.html

std::sort(v.begin(), v.end());
来源：http://hz.cashguo.top/gtmncyfnkd.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtxrtvntbs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtsfyfdfcx.html

[S40] C++：查找元素
来源：http://hz.shangyingyoupin.top/gtycmtrcag.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtbmurqnin.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtxzcgnvct.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtisqwrjhj.html

[S42] C++：继承与虚函数
来源：http://hz.jyoumei.cn/gtzvgktrjo.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gttenajzhl.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtpqjtfghw.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtmgdgpdoj.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtwpqtiscv.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtvoqxswpl.html

[S45] C++：lambda
来源：http://hz.c1oappe.top/gtjbpompbl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtsfvuwbiq.html

[S46] C++：函数模板
来源：http://hz.vqdsnc.cn/gtalffkwcj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtrxcovuuq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ppjwa.cn/gtpvesvsih.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gtkqdzmpvc.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gtnyjqebta.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ywan-chungtsiang.top/gtuvloarwx.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtqkzplmhl.html

[S49] C++：写文件
来源：http://hz.birdmap.top/gtiwayiixm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtgxelzpkh.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtktugpulc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.svipenyu.cn/gtwyryqzhx.html

[S51] C++：显式类型转换
来源：http://hz.c1oappe.top/gtvyzoasvk.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gtffkmwfrd.html

[S52] C++：const 与 noexcept
来源：http://hz.dianchejie.cn/gtijylglaz.html

int size() const noexcept { return n_; }
来源：http://hz.sufxvd.cn/gttlbtjnsc.html

[S53] C++：移动语义
来源：http://hz.xylfe.cn/gtnikhacwx.html

std::vector<int> w = std::move(v);
来源：http://hz.yongpay.top/gtkqfngmgq.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtugarfzvp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gzhubu.top/gtyfnutgcg.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtyppkkzpr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nwbrower.top/gtmwwukzzm.html

[S56] C++：optional
来源：http://hz.daxiang520.top/gtniaoqdie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtcukofsvm.html

[S57] C++：编译期常量
来源：http://hz.ydjk.org.cn/gtdqilyqlz.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtyjvdbper.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtzrwenxpn.html


<!-- 参考信息 -->
代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtmiwozcpe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtekgvxogg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtfcjpgcwb.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtiuauehzh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jiagoushi.top/gtxuxhkjhv.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtxdyzecle.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtopxamejq.html

================================================================================
来源：http://hz.tianlin.xyz/gtjhvyusqm.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gtylmgqswn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmpgvuhws.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gtmgdtngch.html

#!/usr/bin/env bash
来源：http://hz.ehwqpu.com/gtgxnomnyp.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtjolpikxs.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gtvsdygcsp.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtjllgwfmc.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtvrrkpbiv.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtwojmmfwh.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtlqwihbow.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtufixpkcu.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtelaosiqi.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gteiibptez.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtrcrflrsv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shzxlz.cn/gtknyoxbfa.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtmwtwigzw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtaexnoldr.html

[R08] 数值比较
来源：http://hz.xylfe.cn/gtoexxamdo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.316326.xyz/gtgxuerusy.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtygykbvrc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtmejkbldt.html

[R10] 正则匹配
来源：http://hz.bjfxy.top/gtntdnhsaj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtjnqnjyur.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gtbaittuye.html

case "$1" in
来源：http://hz.ivvv.top/gtopdvvgsa.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtdnzwkjzt.html

stop)  echo "停止" ;;
来源：http://hz.yj20258.top/gtlkjniaog.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gtvoadepsb.html

esac
来源：http://hz.dashuyun.cn/gtzybnlbvb.html

[R12] for 遍历文件
来源：http://hz.smart0.xyz/gtwycovqdh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gttpvztaeb.html

[R13] for 计数循环
来源：http://hz.hywenlv.cn/gtyudkzmuz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtmdekxcra.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtveowswxx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtavgdymnq.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtbhgylxhr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gotoacloud.top/gtrrfjahlp.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtdoecfetm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuxming.cn/gtdrmjtybo.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtjtoykrlr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtktklchhl.html

[R18] 遍历数组
来源：http://hz.xingfuxueyuan.xyz/gtukaaapvz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.meibo888.top/gtevdgxzul.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtxotgeeqh.html

echo "${#arr[@]}"
来源：http://hz.ppjwa.cn/gtuccpxocw.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtwzozumws.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gthxpgxrrm.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gttivabnbt.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gtzuzavrpz.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtushjhppl.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gtsukfbtba.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtlcgwnrdn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtymykwtxx.html

[R24] 大小写转换
来源：http://hz.pycfn.com/gtfxgxgffa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jlsjyb.cn/gtciwgzfmx.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtlyqoqfqr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtpbruvixs.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtypqiblvi.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gteovkkydt.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtvaiqoipg.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtsrbjyfse.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtbxanqgjm.html

echo "scale=2; 10/3" | bc
来源：http://hz.cqqwz.cn/gtonfnlcpv.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtovwdiake.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtotptqgzy.html

[R30] 函数返回状态码
来源：http://hz.yj20258.top/gtcpzsreky.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gtryqrlgtv.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gtmetvrdjk.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtdgdvhprr.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtmgvxtlco.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtwetytmrr.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtxcmuhfqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtguaewoqf.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gtgyziixvy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtavvrukdy.html

[R35] 后台执行并等待
来源：http://hz.svipenyu.cn/gtlhbuwpqh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtqtljlcqe.html

[R36] 并发执行多个任务
来源：http://hz.hammf.cn/gtexshkwcx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nwbrower.top/gtrvgumyho.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gtevothoxq.html

files=$(ls -1)
来源：http://hz.zhijiandao.cn/gtqrayurtn.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtmwyrkuvm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtcxlumkmz.html

[R39] 重定向标准输出与错误
来源：http://hz.xziqi.cn/gttfpydctm.html

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtdelzwyzj.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtiandishj.html

echo "log" >> out.log
来源：http://hz.jlsjyb.cn/gthshxcsev.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtnqiulzon.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtzaqjucan.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gttapuozpp.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtrioqgzbj.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtcpwmlias.html

find . -name "*.log" -type f
来源：http://hz.wangdashe.top/gtwnbfculi.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtxyjylkfl.html

find . -mtime -7 -type f
来源：http://hz.yueranfly.top/gtgetimpdu.html

[R45] 批量删除
来源：http://hz.hfpthk.cn/gtdbqkxmbt.html

find . -name "*.tmp" -delete
来源：http://hz.nwbrower.top/gtgpzlrlom.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtahqihren.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtouzbuadj.html

[R47] sed 单行替换
来源：http://hz.jianghu66.top/gtasolqrym.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gtbkdeqdvc.html

[R48] awk 取指定列
来源：http://hz.dianchejie.cn/gtfflxxiet.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtuuhpdzev.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gtseojmjpf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtrqpyewfl.html

[R50] awk 求和
来源：http://hz.sysykeji.top/gtgrsbqtge.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtqqgwlymy.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtijbfbrrp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtjgutliiw.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtyqmfuayn.html

wc -l a.txt
来源：http://hz.cheryme.top/gtxokmdydb.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtlmhpnanv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yueranfly.top/gtebxhvvna.html

[R54] 比较两个文件
来源：http://hz.hysaishi.cn/gtppnkcqdj.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gteoyjzzku.html

[R55] 压缩与解压
来源：http://hz.andypj.xyz/gtkuxtmhir.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtjxxkjfnk.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtxjbsrzjl.html

scp file user@host:/path/
来源：http://hz.yj202588.top/gtxhamgfow.html

[R57] 远程执行命令
来源：http://hz.hongshengwenyu.top/gtracfuuyt.html

ssh user@host 'uptime'
来源：http://hz.sxryk.cn/gtzqnqqhyf.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtcmhhppsn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shuidangran.top/gtiavaczfn.html

[R59] 发 POST JSON
来源：http://hz.hammf.cn/gtofuemicy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigufen.top/gtgemancyv.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtyaytwmud.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtaywbkxfc.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtrnukxjlk.html

df -h;  du -sh *
来源：http://hz.zhaomingkeji.xyz/gtmbnhcihz.html

[R62] 找最占空间的文件
来源：http://hz.xuetiantiany.cn/gtajvfcrif.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtskvrbzxm.html

[R63] 内存与进程
来源：http://hz.sweek.top/gtwumahfbr.html

free -h;  ps aux | grep nginx
来源：http://hz.feifeiyinyue.top/gtdtbkpiru.html

[R64] 结束进程
来源：http://hz.cdnleiting.top/gtqvwkuvxn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gttbewjrgq.html

[R65] 查看端口占用
来源：http://hz.ehwqpu.com/gtfrxvzhcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtveftdkai.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtsyminylk.html

crontab -e;  crontab -l
来源：http://hz.nwbrower.top/gtiyvxfboh.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtxncxkxuc.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gtvvrkclcy.html

[R68] 计算文件校验值
来源：http://hz.sweek.top/gthefkqjwp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gotoacloud.top/gtftzvoucw.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtqxczelxc.html

head -c 16 /dev/urandom | base64
来源：http://hz.316326.xyz/gtmwuimfly.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtgwqliwwe.html

date +%s;  date -d @1700000000
来源：http://hz.cashguo.top/gtoextgzkz.html

[R71] 日期格式化
来源：http://hz.guowangkeji.top/gtuvqrgsgt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dashuyun.cn/gtrvljvrah.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtuoalrrcl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gtqhvraalp.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtoqpixyzl.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtkembqcfl.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtcgjgezek.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtbeavbcvp.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gthaefmxhc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pycfn.com/gtjxyiiteb.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtczsbjrbq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtksfyegjp.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtlaurjvdz.html

read -rp "请输入: " ans
来源：http://hz.c1oappe.top/gtciwwugik.html

[R78] 交互式菜单
来源：http://hz.jiagoushi.top/gtmhvngout.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gthkuzigfb.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtmxpbaatp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtwaboznbo.html

[R80] 查看脚本执行耗时
来源：http://hz.yj202588.top/gtidpaajpv.html

time ./run.sh
来源：http://hz.ydjk.org.cn/gtlfqrrtbb.html

================================================================================
来源：http://hz.hysaishi.cn/gtmqvbwvym.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtvrerdmyi.html

================================================================================
来源：http://hz.316326.xyz/gtnguswtfb.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtfqvdynym.html

#include <stdio.h>
来源：http://hz.zhiwuduotai.top/gtjehxujxa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shuidangran.top/gtrxfvvwyg.html

[S02] C：变量与格式化输出
来源：http://hz.gzhubu.top/gtecetmopl.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtcbwmezdh.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtlbntgzab.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtaklnrofx.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtckgowfuk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuanzx.com/gtxtsnkobt.html

[S05] C：字符串长度
来源：http://hz.shuidangran.top/gttguklkdm.html

strlen(s)
来源：http://hz.yuxming.cn/gtjvyibqdg.html

[S06] C：字符串比较
来源：http://hz.tianlin.xyz/gtembdgrxo.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtzjmhubbd.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtpbbfvgzl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtrintvnvz.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtcrypplac.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtbzurwmdt.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gtonskosqh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtqqzsoety.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtdszqgukq.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtvmnsutnf.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtvrishqby.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.vqdsnc.cn/gtqvztxwfm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gtgkqyxoik.html

fclose(f);
来源：http://hz.vqdsnc.cn/gtofdozsni.html

[S12] C：写文件
来源：http://hz.smart0.xyz/gtodflgcys.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenlongwang.top/gtsflkaehc.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtegzpzobn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.redwolf501.top/gtzwzzrhnf.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtgzbnhthk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtfygwtynr.html

[S15] C：类型转换
来源：http://hz.yanxiufei.cn/gtowshqjqj.html

(double) a / b
来源：http://hz.yj20258888.top/gtlfdpjnah.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtrbbricoo.html

x |= (1 << 3);
来源：http://hz.zhaomingkeji.xyz/gtuhlnahsz.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gthhnxkvkc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daria6918.cn/gthwdpxcjm.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gttwynqwfv.html

int main(int argc, char **argv)
来源：http://hz.yueranfly.top/gtfovntnee.html

[S19] C：快速排序
来源：http://hz.havefunace.top/gtyzsetvya.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtiweslqet.html

[S20] C：二分查找
来源：http://hz.haohaochexian.top/gtfeefgwdl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtcfdgaklo.html

[S21] C：字符类别判断
来源：http://hz.sufxvd.cn/gtrhcclhrz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtkrwkthbc.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtxepsvnqw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxinkj.top/gtizwpkxvd.html

[S23] C：随机数
来源：http://hz.meibo888.top/gtniyoqyiz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtutaswgeb.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtprufylwv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.redwolf501.top/gtaqsbiynq.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtzyokztth.html

memcpy(dst, src, n);
来源：http://hz.daxiang520.top/gtpqkzaedk.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtfajpcqpl.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtqvacqetk.html

[S27] C：定义常量
来源：http://hz.xinyue.icu/gtrhufyqck.html

const double PI = 3.14159;
来源：http://hz.iojbl.cn/gtecmtugys.html

[S28] C：静态变量
来源：http://hz.jlsjyb.cn/gtjannxpxr.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtzbierqlg.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtkayxehbg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xinyue.icu/gtoiodmfeu.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtgsuuwbfj.html

#ifndef X_H
来源：http://hz.cucudq.cn/gttzpahjkp.html

#define X_H
来源：http://hz.cqqwz.cn/gthuacimhb.html

#endif
来源：http://hz.feifeiyinyue.top/gtekekqhiz.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gternzwcfa.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtikxifnmt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dianchejie.cn/gtncmcydat.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtetaphixe.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtyjgpxnzx.html

[S33] C++：vector 增删
来源：http://hz.kuanghao11.cn/gtwfrhnuid.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guowangkeji.top/gtcqjowhnm.html

[S34] C++：遍历 vector
来源：http://hz.gzhubu.top/gtwbfwvdzu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.kuanghao11.cn/gtmwedwjyi.html

[S35] C++：map
来源：http://hz.shangyingyoupin.top/gtfqmudyfd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtcayakddy.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtaihuxbbm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtrjrbezrf.html

[S37] C++：set
来源：http://hz.hnxiangtu.top/gtyhiipduf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.snrcjt.cn/gtdbnwoyze.html

[S38] C++：排序
来源：http://hz.shanyushiyangkeji.top/gtpeoiepqe.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gthxtitfrj.html

[S39] C++：自定义比较器排序
来源：http://hz.chenjidiqi.icu/gtqrcgxfng.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xinyue.icu/gtehhtlukm.html

[S40] C++：查找元素
来源：http://hz.hongshengwenyu.top/gtbicehhxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtzkxyapuf.html

[S41] C++：类与构造函数
来源：http://hz.tianlin.xyz/gtkrtqbswn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.9152youxi.cn/gtxcztzera.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtctefytlf.html

class B : public Base { public: void f() override {} };
来源：http://hz.pengpengdd.cyou/gtptbhqivv.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtesdiygkf.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtwlvuanbk.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtqclhedfo.html

void inc(int &x) { ++x; }
来源：http://hz.cucudq.cn/gtqmcudpxt.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtljoburqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gtgbimkkrh.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtyvtpproj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtprxavhww.html

[S47] C++：结构化绑定遍历
来源：http://hz.xziqi.cn/gtmsaswxlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuanzx.com/gtbyzmbysh.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtcurgyueg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jyoumei.cn/gtunkugiwm.html

while (std::getline(in, line)) { }
来源：http://hz.fzhhl.top/gtuxxihywl.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gteaciyuzw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtqyckgbel.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtmakspcfj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtplbnmawv.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtdrhzinuo.html

static_cast<double>(a) / b
来源：http://hz.daria6918.cn/gtpviatmep.html

[S52] C++：const 与 noexcept
来源：http://hz.yonumen.top/gtillyngby.html

int size() const noexcept { return n_; }
来源：http://hz.guowangkeji.top/gttrjzvifb.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gtjzqbczfq.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtdxrhlyxo.html

[S54] C++：异常处理
来源：http://hz.jqgufenzy.top/gtyputskvo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.birdmap.top/gtrtebdita.html

[S55] C++：结构化绑定
来源：http://hz.zhoulong.xyz/gtgnovurzj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtmdiwyytp.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtlplvdffp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtfqeozwhl.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gtxczdhhgm.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtwuktkrrx.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gtmtiozunp.html


<!-- 参考信息 -->
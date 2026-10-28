代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gthwpamtdo.html

SELECT TRIM(name) FROM users;
来源：http://hz.dashuyun.cn/gtkyzfsaob.html

[Q85] 数值取整
来源：http://hz.cheryme.top/gtvuyqnbat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gzhubu.top/gterryoceo.html

[Q86] 读取 JSON 字段
来源：http://hz.havefunace.top/gtczksxqxd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.mhx1999.top/gtabijaqzv.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gtxataykri.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtnxjbbnpm.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtpjsvvngo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gthgrevqkx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.havefunace.top/gtvairhtsy.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtkpuvmtsz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.redwolf501.top/gtqkqgohqo.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtxydsusdt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtwduxxlha.html

================================================================================
来源：http://hz.yonumen.top/gtmlmdwbfo.html

R. Bash 专题
来源：http://hz.wangdashe.top/gtfxudkwso.html

================================================================================
来源：http://hz.aizwys.cn/gthtfbizjp.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtyiowwabm.html

#!/usr/bin/env bash
来源：http://hz.gogol.net.cn/gtqawnivur.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtsifabnok.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtkoqapqnh.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtbpjkgghd.html

[R03] 只读变量
来源：http://hz.0kj1m.cn/gtnjxkkbdq.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtxeqrnpsi.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtzaynvzzf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.316326.xyz/gtihdnspgk.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtuaqsowxd.html

name="${1:-default}"
来源：http://hz.yangfankeji.com/gthvfvmjzl.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtvacidlbd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tanke756.top/gtxgwzpjbp.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gttgzvurxb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtwdwrgbri.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gthgswtjxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gtasyzsumf.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtkhmkjagf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtjfddkqvk.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtxxcwvizh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtfprariip.html

[R11] case 多分支
来源：http://hz.jinghuilouyu.cn/gtnyuombew.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtpvxhgyxp.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gttfmkzfgy.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtljmaxonu.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtiyqdfnuy.html

esac
来源：http://hz.smart0.xyz/gtuwrwqfmm.html

[R12] for 遍历文件
来源：http://hz.jianghu66.top/gtitpvsalj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gtplscklzo.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtcpumlkie.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtvfffrpiw.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtjnqivmvn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtkwrudsei.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gthvaoidjl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ppjwa.cn/gtftjknhgi.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtpyofxppd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigufen.top/gtazqnilfv.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtooghmrll.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtfzsfcyqp.html

[R18] 遍历数组
来源：http://hz.zhiwuduotai.top/gtukunjkzo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtbxwzfghs.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtjoknidxv.html

echo "${#arr[@]}"
来源：http://hz.xingfuxueyuan.xyz/gtwuvqdowe.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gttdzalzzg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.feifeiyinyue.top/gtdiblnoul.html

[R21] 字符串长度
来源：http://hz.jlsjyb.cn/gtdkhsqvcv.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtfnfdpibj.html

[R22] 截取子串
来源：http://hz.yj20258888.top/gturnumeeh.html

echo "${s:0:5}"
来源：http://hz.shuidangran.top/gtywpjvhrt.html

[R23] 字符串替换
来源：http://hz.yongpay.top/gtcijylcyr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gzhubu.top/gtdmaaaavz.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtkjbhemdj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sweek.top/gtaeftekwo.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnxiangtu.top/gtdqnjmoqu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jianghu66.top/gtrxirqagz.html

[R26] 命令替换
来源：http://hz.cdnleiting.top/gtcafpxgst.html

now=$(date +%F); echo "$now"
来源：http://hz.xziqi.cn/gtmawowpbf.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtpismeltk.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtrdufrjzx.html

[R28] 浮点运算
来源：http://hz.gaohongyu789.top/gtzazlsrln.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtaxpzrhck.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtbyqeklbq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtkyibmaau.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtflzwxisp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ivvv.top/gtavoioaof.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtqnvtawjb.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtuyqvbxrq.html

[R32] 参数个数校验
来源：http://hz.ybcxt.top/gtfzbojspl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shzxlz.cn/gtnkrbkltz.html

[R33] 捕获错误并提示行号
来源：http://hz.feifeiyinyue.top/gtswgfievt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtzuclawpo.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gtvnewfoug.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtswtaoyxn.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtcbrpueav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtseiulnsc.html

[R36] 并发执行多个任务
来源：http://hz.svipenyu.cn/gtvhyiwjlb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtovsjeuws.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtspblkcmc.html

files=$(ls -1)
来源：http://hz.52xcode.cn/gtschqohwq.html

[R38] 管道串联
来源：http://hz.ybcxt.top/gtbgimyczy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtzezsbaow.html

[R39] 重定向标准输出与错误
来源：http://hz.havefunace.top/gtrrttkcrx.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gttwqebmpu.html

[R40] 追加写日志
来源：http://hz.xylfe.cn/gtrxegoiyp.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtcwmhkjnb.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtgpegwqhw.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gttsurozpa.html

[R42] 输入重定向
来源：http://hz.jlsjyb.cn/gtxqssztlr.html

wc -l < a.txt
来源：http://hz.quarkkingdee.top/gttdpxsdga.html

[R43] 按名字查找文件
来源：http://hz.yueranfly.top/gtmfnkhllo.html

find . -name "*.log" -type f
来源：http://hz.ydjk.org.cn/gtgkubwfhi.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtfkhbktky.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gtqopnpieu.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtzvqxiyrs.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtjsbotcod.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gtrnhvqoxv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtfwcetmsh.html

[R47] sed 单行替换
来源：http://hz.nanxinkj.top/gtsuyyjrto.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gzhubu.top/gtdkggsbyh.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtdlodydms.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtkywebykf.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtiuuugvxi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tian-w.cn/gtajgmrtpe.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtvhhdadya.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtbyignpfu.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangkeji.top/gtrpysqfqo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtmbtmbeoa.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtpspwbmeh.html

wc -l a.txt
来源：http://hz.tanke756.top/gtqucfwjad.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtajcpatpi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtcjcbtcnj.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtydskqsnj.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gtixmhqvlw.html

[R55] 压缩与解压
来源：http://hz.ehwqpu.com/gtuxbltjzz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgufenzy.top/gtqtnqlzud.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtnxiqknkx.html

scp file user@host:/path/
来源：http://hz.jyoumei.cn/gtsigckikk.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtruqealyd.html

ssh user@host 'uptime'
来源：http://hz.ywan-chungtsiang.top/gtlctgafvi.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtciiptros.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yueranfly.top/gtjasepukl.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtcssbpxun.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenzaomai.com/gtfuzpjmnz.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydzc1.top/gtwesssasu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtyjundlfk.html

[R61] 磁盘占用
来源：http://hz.yuxming.cn/gtfwbcygem.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtomeasioa.html

[R62] 找最占空间的文件
来源：http://hz.tianlin.xyz/gtkxchomzx.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtwylbzwoj.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtvfsfgrqg.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtsaasqhvg.html

[R64] 结束进程
来源：http://hz.xingfuxueyuan.xyz/gtxcrlgsof.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtchzigzak.html

[R65] 查看端口占用
来源：http://hz.fzhhl.top/gtfgavqtot.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtnzhnkdth.html

[R66] 定时任务
来源：http://hz.birdmap.top/gtxywzkwaq.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtzolcqnws.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtovkoddfa.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtjrctwwtg.html

[R68] 计算文件校验值
来源：http://hz.xingfuxueyuan.xyz/gtehwqfqze.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.vqdsnc.cn/gtryhptioo.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gtggmzjhzn.html

head -c 16 /dev/urandom | base64
来源：http://hz.yanxiufei.cn/gtwwzpkaxn.html

[R70] 时间戳与互转
来源：http://hz.vqdsnc.cn/gtniixkfnd.html

date +%s;  date -d @1700000000
来源：http://hz.zhijiandao.cn/gtqncsonbv.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtqavvjvhk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tanke756.top/gtwojuidzs.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtrziiruqs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuxming.cn/gtihsjwslz.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtzgwvzdrr.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtghnqivdv.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtcwewhhqw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtfbahxstu.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtnazkhpqi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinghuilouyu.cn/gtgzqlmoeo.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtgoazoucn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtcsxgoxdy.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtjnxzbwaw.html

read -rp "请输入: " ans
来源：http://hz.dashuyun.cn/gtpakmtjqj.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtzmxizvag.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gtdtfgytyz.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtowheercs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtofjutjfe.html

[R80] 查看脚本执行耗时
来源：http://hz.0kj1m.cn/gtapsduqma.html

time ./run.sh
来源：http://hz.shuidangran.top/gtxxkkehnd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuqyponuv.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtkcljpgsv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqcdsmudx.html

[S01] C：Hello World
来源：http://hz.birdmap.top/gtawnjjaxm.html

#include <stdio.h>
来源：http://hz.xziqi.cn/gtuscaguhx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtdhsciipp.html

[S02] C：变量与格式化输出
来源：http://hz.tianlin.xyz/gtmyisxugn.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtuzbznyqm.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtkvzdahpr.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtjajcychr.html

[S04] C：字符串复制
来源：http://hz.bjfxy.top/gtfomifxaj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtambydcgi.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gttwycalcw.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gttcercnbl.html

[S06] C：字符串比较
来源：http://hz.zhiwuduotai.top/gtfxzzjxbh.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtiffldtjw.html

[S07] C：数组遍历求和
来源：http://hz.gogol.net.cn/gtdwmshwkq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtwpshhcyx.html

[S08] C：动态内存分配与释放
来源：http://hz.zycfv.cn/gtlqmytxcl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258888.top/gthsfiziay.html

[S09] C：结构体定义与初始化
来源：http://hz.daxiang520.top/gtpuwmhwkc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangshuangyany.cn/gtvyvjmbmy.html

[S10] C：指针与解引用
来源：http://hz.yanxiufei.cn/gtzjbzqyzn.html

int *p = &a;  *p = 5;
来源：http://hz.redwolf501.top/gtgvixlewg.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtqlzisqwk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gtliaenwff.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtawjgwprc.html

fclose(f);
来源：http://hz.c1oappe.top/gtznqpokwu.html

[S12] C：写文件
来源：http://hz.ppjwa.cn/gtctqyndiz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fzhhl.top/gtqkiwdobv.html

[S13] C：宏定义
来源：http://hz.zhixingplan.top/gtrphazolb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xingfuxueyuan.xyz/gtwdigtwvn.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtbszbbcbf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtyolkvfhr.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gthphfmwgm.html

(double) a / b
来源：http://hz.hfpthk.cn/gteiovfjkf.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtuteknvcq.html

x |= (1 << 3);
来源：http://hz.shanyushiyangtech.top/gttpyhwkrw.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gtmueluhxx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtoerkdftp.html

[S18] C：命令行参数
来源：http://hz.birdmap.top/gtlxqyxjzm.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtoulgsjlo.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtepmwbjxu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtsiyjkydh.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtcwjyujnt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtwuwxfbue.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gttwfnqfwt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhengqikj.top/gtxcbwwuwo.html

[S22] C：字符串转数字
来源：http://hz.wangdashe.top/gtulhqmdyy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtyibjylfn.html

[S23] C：随机数
来源：http://hz.meibo888.top/gtzpagpusb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnqzz.top/gttlfkousc.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtpalvtlqv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guannengcc.top/gtphdobgri.html

[S25] C：内存拷贝
来源：http://hz.c1oappe.top/gtkmmafnex.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtzmxcszqa.html

[S26] C：内存清零
来源：http://hz.zycfv.cn/gtwyzajfpa.html

memset(a, 0, sizeof a);
来源：http://hz.daria6918.cn/gteqbjjirm.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtvuwaaphn.html

const double PI = 3.14159;
来源：http://hz.ydzc1.top/gtbuxcpptk.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtfkxtspab.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtkgzhxoov.html

[S29] C：变参函数
来源：http://hz.nanxuanxn.top/gtfpnisqzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ybcxt.top/gtvmmjfrlx.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gtmahsuhfv.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtoxmagoge.html

#define X_H
来源：http://hz.tanke756.top/gteabyxakz.html

#endif
来源：http://hz.hfpthk.cn/gtsjyuvtvm.html

[S31] C++：Hello World
来源：http://hz.yuanzhike.top/gtdrzpoabr.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtctoetnhm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtygfcytyk.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtchepwlnm.html

std::string s = "hi";  s += "!";
来源：http://hz.gotoacloud.top/gtddmhaibw.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gttwuckcdq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtvezdvgto.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtnwdvnwko.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtvukbdgaj.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtytcgddkt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtmevzkxug.html

[S36] C++：unordered_map
来源：http://hz.aizwys.cn/gtvhtgnvgg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtbqgtcqjd.html

[S37] C++：set
来源：http://hz.hnxiangtu.top/gtcbevtyks.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.mhx1999.top/gtcliyuwcf.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtysftlgpp.html

std::sort(v.begin(), v.end());
来源：http://hz.xylfe.cn/gtodxjapkk.html

[S39] C++：自定义比较器排序
来源：http://hz.dianchejie.cn/gtgdjjkstj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtmkdedadu.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtxapvdsyj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtwiryrlwk.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtqtpxgpey.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtmgyrwfih.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtpvxbfasj.html

class B : public Base { public: void f() override {} };
来源：http://hz.316326.xyz/gtotwwdbhu.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtmgotlmfi.html

auto p = std::make_unique<int>(5);
来源：http://hz.redwolf501.top/gtjqjcjoyp.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtmyjzzyic.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtlzutkdwp.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gttijkarzy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtbxndicor.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtlijbeidp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtjsfcxjna.html

[S47] C++：结构化绑定遍历
来源：http://hz.sweek.top/gtgzrwgith.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtkxezffmi.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtvkjruhcx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pycfn.com/gtsrcacjzw.html

while (std::getline(in, line)) { }
来源：http://hz.ybcxt.top/gtfnlbsctt.html

[S49] C++：写文件
来源：http://hz.hongshengwenyu.top/gtncdbktiu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gzhubu.top/gtsihmvfma.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtsvqeyopt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangshuangyany.cn/gtdxwkhlmp.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtnmixlupa.html

static_cast<double>(a) / b
来源：http://hz.gaohongyu789.top/gtooyzatsz.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gttmhmrblr.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtbbiwjgit.html

[S53] C++：移动语义
来源：http://hz.guowangkeji.top/gtvecezwkv.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtldkabdly.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtvyfhdxwn.html


<!-- 参考信息 -->
代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.0kj1m.cn/gtebsqrvmd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtwjvvfjtm.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtmihzkokh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtqrxxsoly.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gtjwwhfzds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtszmpbjnp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cashguo.top/gtkvgrdntc.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtgfgrmlac.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aizwys.cn/gtcdgwhyna.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtuvmelhtn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtwnnfnsej.html

================================================================================
来源：http://hz.hammf.cn/gttvuntkjn.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gthipvfiob.html

================================================================================
来源：http://hz.sysykeji.top/gtnojzqpim.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtqohhrpel.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gtobhnjycv.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtwwdjxtwq.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtuuzgfttb.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtqkltnphy.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtvmqfqrtu.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtjbernidn.html

[R04] 位置参数
来源：http://hz.ivvv.top/gthwpxhyxw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxuanxn.top/gtapyngext.html

[R05] 参数默认值
来源：http://hz.gotoacloud.top/gtwjqyxexx.html

name="${1:-default}"
来源：http://hz.yanxiufei.cn/gthuoosxsz.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtgqpasazt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gzhubu.top/gtxvwzuvuo.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtssyinmos.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtsiihjhsj.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gttzheswhr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guannengcc.top/gtgyrmqkjl.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gtoqxfapxk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhongyouzk.top/gtelxjulvu.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gtigoyghhz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhijiandao.cn/gtdtmjtwhr.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtrdzbljun.html

case "$1" in
来源：http://hz.dianchejie.cn/gteofpyjbf.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtmgeblzkx.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtniiwchdk.html

*)     echo "未知命令" ;;
来源：http://hz.zhixingplan.top/gtxbwjdrnd.html

esac
来源：http://hz.sxryk.cn/gtzoeznvzh.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtplbghwhw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.316326.xyz/gtonjjsvfp.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gttzzrgpdr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dashuyun.cn/gtdsgksjaw.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtzxorcpan.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtyfdwgdbb.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtoedfmuzs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinyuanbaomall.cn/gtsckalxch.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gtiwltvrcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtmfdtjhhi.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gtsdiujlii.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenzaomai.com/gtwwjvccgk.html

[R18] 遍历数组
来源：http://hz.zycfv.cn/gtasucavkh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj202588.top/gtoghsgaol.html

[R19] 数组长度
来源：http://hz.nanxinkj.top/gtkegpndop.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtkrbpptre.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtpdxhrrdu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhiwuduotai.top/gtsskwtngz.html

[R21] 字符串长度
来源：http://hz.yonumen.top/gtzimbwwiu.html

echo "${#s}"
来源：http://hz.hammf.cn/gtfeibccmf.html

[R22] 截取子串
来源：http://hz.yuxming.cn/gttjtcqgdh.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtchndiqca.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtllaegjzh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtterdalxf.html

[R24] 大小写转换
来源：http://hz.dashuyun.cn/gtaqvlpxwb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydzc1.top/gtfynwjbtt.html

[R25] 去后缀 / 去前缀
来源：http://hz.guannengcc.top/gtiizsoesy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xziqi.cn/gtjyckhojc.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtriubtjjp.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gticygsawe.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtcerhuzwl.html

echo $((1 + 2 * 3))
来源：http://hz.yvedp.cn/gtrqhmdtrl.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtribhjttr.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgfzy.top/gthmmtemqv.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtmwtzyccm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuetiantiany.cn/gtxgfrzkpo.html

[R30] 函数返回状态码
来源：http://hz.wangshuangyany.cn/gtqtbylxvk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gtninsqkif.html

[R31] 局部变量
来源：http://hz.haohaochexian.top/gtfawwusfi.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinghuilouyu.cn/gteheiojhj.html

[R32] 参数个数校验
来源：http://hz.birdmap.top/gtdgkpwsob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aizwys.cn/gtzitsdwmv.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtivqngqde.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yongpay.top/gtsfkpxjbo.html

[R34] 退出时清理
来源：http://hz.mhx1999.top/gtzqwzfxay.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtphxfbyai.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtpriaibwv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daxiang520.top/gtmrvisvrv.html

[R36] 并发执行多个任务
来源：http://hz.pengpengdd.cyou/gtkemvudbq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gotoacloud.top/gthlzjrqkp.html

[R37] 把输出赋给变量
来源：http://hz.hysaishi.cn/gtknvscdzy.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtsiwcvfsm.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gttpywxgzt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtuosukxrc.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gtjmuqdcnj.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtpiweuspy.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtkwdfzzfh.html

echo "log" >> out.log
来源：http://hz.yj20258888.top/gtyalmzwgr.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gtuwzynbqk.html

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gttdqdawwy.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtmdycfamn.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtcskcywin.html

[R43] 按名字查找文件
来源：http://hz.chenjidiqi.icu/gtvtdspaow.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtomqhaigr.html

[R44] 按修改时间查找
来源：http://hz.hongshengwenyu.top/gtbamrvtsw.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtstbsffnl.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtxytcssmw.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtgdapiuws.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtbxhbzzvi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtrvheceim.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtelvdzvjx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtclewobqn.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtealoiipy.html

awk '{print $1, $3}' a.txt
来源：http://hz.guowangkeji.top/gtnijyvhby.html

[R49] awk 带条件
来源：http://hz.guowangkeji.top/gtefgqhbxq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenlongwang.top/gtljjfddvg.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtzbrqsgom.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtnjbtonvg.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtekcxppev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.havefunace.top/gtlvdadyiq.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtpdlabtpc.html

wc -l a.txt
来源：http://hz.chenjidiqi.icu/gtwwmadhtm.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gtofmeesws.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhixingplan.top/gtzhsnxwnv.html

[R54] 比较两个文件
来源：http://hz.nanxuanxn.top/gtpwqbnuzu.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtaqknpgte.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtmehhczvy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtzbmmbiyj.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtfonauwdg.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtdhsjehdp.html

[R57] 远程执行命令
来源：http://hz.nanxuanxn.top/gtdmwovfay.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gttaupojmr.html

[R58] 下载文件
来源：http://hz.fengsongda.top/gtoqioealj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ppjwa.cn/gtdphxblkr.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtxetvnasm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gtqepswvya.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtxefpemwa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtngvamziz.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtnhkxkihb.html

df -h;  du -sh *
来源：http://hz.snrcjt.cn/gtzzxrmbnl.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtshtrulxx.html

du -ah . | sort -rh | head -10
来源：http://hz.xinyue.icu/gtmvgkawle.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtvicwafpf.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtyoflqpwu.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gthljbftob.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtmgvjjoxa.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtbjkfhxhe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.0kj1m.cn/gtrqabmkwy.html

[R66] 定时任务
来源：http://hz.tian-w.cn/gtqvvbaznt.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtpykoxtwt.html

[R67] 生成随机十六进制串
来源：http://hz.yongpay.top/gtzjusehil.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gthgrbhgyt.html

[R68] 计算文件校验值
来源：http://hz.hfpthk.cn/gtfypaszmt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtobnwyckj.html

[R69] 生成随机密码
来源：http://hz.guowangkeji.top/gtliyxhwfm.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtrlxhzjqz.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtrdaeidii.html

date +%s;  date -d @1700000000
来源：http://hz.c1oappe.top/gttqrtsegl.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtcqmdeihc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtgoupbhbj.html

[R72] 等待端口就绪
来源：http://hz.yonumen.top/gthpxxyqmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtxztbvnnh.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtkvumlaux.html

split -l 1000 big.log part_
来源：http://hz.jlsjyb.cn/gtxnatrhle.html

[R74] 批量重命名
来源：http://hz.ydjk.org.cn/gtnemxomzp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangdashe.top/gtaynouhqc.html

[R75] 导出环境变量
来源：http://hz.hysaishi.cn/gtyixjctbw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gtdmticlqj.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtgjtqvsrs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtqugcaown.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtifkaopam.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtbvhfsepl.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtxusrjcfn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gtzbwhpeih.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gtejsfmund.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nwbrower.top/gtcubbuppe.html

[R80] 查看脚本执行耗时
来源：http://hz.yuanzhike.top/gtuhortdtd.html

time ./run.sh
来源：http://hz.bjfxy.top/gtjunadclv.html

================================================================================
来源：http://hz.cashguo.top/gtomikkert.html

S. C / C++ 专题
来源：http://hz.fengsongda.top/gticbdajgn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtrnndfrgz.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtxnctsekh.html

#include <stdio.h>
来源：http://hz.jqgufenzy.top/gtjudnjygg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtvdqwwpjr.html

[S02] C：变量与格式化输出
来源：http://hz.jiagoushi.top/gtvwojofbk.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangshuangyany.cn/gtibqrkzcb.html

[S03] C：读入整数
来源：http://hz.chenlongwang.top/gtpexhpwct.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtxdjdarca.html

[S04] C：字符串复制
来源：http://hz.ivvv.top/gtyoulyshx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.fzhhl.top/gtyvppkmbg.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtajwvtxsl.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtlxfrsddl.html

[S06] C：字符串比较
来源：http://hz.jlsjyb.cn/gtplmofxwp.html

strcmp(a, b) == 0
来源：http://hz.svipenyu.cn/gtynvcstgl.html

[S07] C：数组遍历求和
来源：http://hz.daxiang520.top/gtkaywpwxj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtfxnzjlbf.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtwcfvchdz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgufenzy.top/gtxsprerdp.html

[S09] C：结构体定义与初始化
来源：http://hz.pengpengdd.cyou/gtsyevzgxu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtuzxkvzrg.html

[S10] C：指针与解引用
来源：http://hz.quarkkingdee.top/gtbbfzequj.html

int *p = &a;  *p = 5;
来源：http://hz.zhaomingkeji.xyz/gtezbkvexr.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtaclcoktm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtbgmeogdd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gttxqbylmh.html

fclose(f);
来源：http://hz.pycfn.com/gtlsctniii.html

[S12] C：写文件
来源：http://hz.wangdashe.top/gtrqgtcqkv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtlkbjvnni.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtxxfoyacf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtylknfkfp.html

[S14] C：枚举
来源：http://hz.jqgufenzy.top/gtanrklkid.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shangyingyoupin.top/gtlafkwkht.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtimbkxojj.html

(double) a / b
来源：http://hz.yuanzhike.top/gtpohgevga.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtxdrfibuv.html

x |= (1 << 3);
来源：http://hz.ydzc1.top/gtrjhivwzt.html

[S17] C：安全拼接字符串
来源：http://hz.ydjk.org.cn/gtbyyiyups.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhiwuduotai.top/gtfyowlxfl.html

[S18] C：命令行参数
来源：http://hz.hysaishi.cn/gttwimpmeg.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtqccrvkah.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gtpbmssqnm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtiwwtnvel.html

[S20] C：二分查找
来源：http://hz.hywenlv.cn/gtujmrfqts.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gtxdvxmjzl.html

[S21] C：字符类别判断
来源：http://hz.hnxiangtu.top/gtfyjfhwlk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuxming.cn/gthyogutdj.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtuhzflnfx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtawxaobxg.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtaldhzzzo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtfjdskjpb.html

[S24] C：获取本地时间
来源：http://hz.jinqigufen.top/gtjnwjgyhe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.9152youxi.cn/gtrtimxenw.html

[S25] C：内存拷贝
来源：http://hz.meibo888.top/gtocfxguoi.html

memcpy(dst, src, n);
来源：http://hz.vqdsnc.cn/gtanyuwezc.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gthssadgrg.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtvtftoslr.html

[S27] C：定义常量
来源：http://hz.ybcxt.top/gtrkqobush.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtuhwbrcfn.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtriukhejh.html

static int counter = 0;
来源：http://hz.cashguo.top/gtrtojwvvp.html

[S29] C：变参函数
来源：http://hz.cdnleiting.top/gthypqwkyw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gtpzyapkwv.html

[S30] C：头文件保护
来源：http://hz.xylfe.cn/gtqstefgjv.html

#ifndef X_H
来源：http://hz.chenlongwang.top/gtfrafpuap.html

#define X_H
来源：http://hz.jinyuanbaomall.cn/gtjlecmyck.html

#endif
来源：http://hz.chenzaomai.com/gtctgezkjp.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gtwphqpasf.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtfrcntuqc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258888.top/gthcgmsvpe.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtbpkrmqay.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtbezstixx.html

[S33] C++：vector 增删
来源：http://hz.daxiang520.top/gtkgaoachh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gtikrmwxok.html

[S34] C++：遍历 vector
来源：http://hz.jiagoushi.top/gtokuibdpt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtdpzanzfc.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtliqwcigk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtfxxsvqar.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtvhijzivb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtexvcjhqo.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtfwvaapoc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtdkrbgbex.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtpssjcaer.html

std::sort(v.begin(), v.end());
来源：http://hz.9152youxi.cn/gtuqalcmev.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtjzwhgiuf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtdygzkkuo.html

[S40] C++：查找元素
来源：http://hz.tian-w.cn/gtoxljxkpd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtjjxydbfz.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtetqzbrnr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtdoyeubqa.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gthblkfwzs.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtfiugqhaj.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtbwwnyqwo.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtduvrajlp.html

[S44] C++：引用传参
来源：http://hz.316326.xyz/gtnlarepju.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangtech.top/gtqdlieurh.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtfpxrzohp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.mhx1999.top/gtfutgiuyg.html

[S46] C++：函数模板
来源：http://hz.jianghu66.top/gtkotirfqj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.316326.xyz/gtemhjzrne.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj202588.top/gtngzboxzt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtpsjjjcus.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gtxyjoyvar.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnqzz.top/gtpgjfsasu.html

while (std::getline(in, line)) { }
来源：http://hz.sysykeji.top/gtosflvpmr.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtndeytcmn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yangfankeji.com/gtbpzpvhsd.html

[S50] C++：格式化数字
来源：http://hz.zhiwuduotai.top/gtqygbkawi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gttlkoxgmh.html

[S51] C++：显式类型转换
来源：http://hz.ivvv.top/gtgtphhwfh.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtweztxtkz.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtizpuxrvh.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtyftmlvra.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gtcjjzgosw.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtgscwzbim.html

[S54] C++：异常处理
来源：http://hz.gaohongyu789.top/gtsxcoklio.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtpnvdnksv.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtnkrbeyle.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtuuffaxfg.html

[S56] C++：optional
来源：http://hz.shanyushiyangtech.top/gtvzrwdktv.html


<!-- 参考信息 -->
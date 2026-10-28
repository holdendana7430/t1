代发 wailian999

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtbakjgxft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtvnkrvpfr.html

[Q81] 字符串替换
来源：http://hz.snrcjt.cn/gtfmdobtfa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cheryme.top/gtbusqijaa.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtslqklnzo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.c1oappe.top/gtaxjeosnq.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtkhjxcntk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtyaqnhnjp.html

[Q84] 去除首尾空格
来源：http://hz.ppjwa.cn/gtcrrjebsm.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtxtbdmyeb.html

[Q85] 数值取整
来源：http://hz.xylfe.cn/gtyqghsxxd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cashguo.top/gtgeydtvnu.html

[Q86] 读取 JSON 字段
来源：http://hz.52xcode.cn/gteadmczef.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangkeji.top/gtjattnogj.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtsarfdddd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenjidiqi.icu/gtgzviztns.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtchbvmhmp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.mhx1999.top/gtjlefvmwo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtjjgkbhiw.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtkhgdoxxp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yueranfly.top/gtkvukyllb.html

[Q90] 生成序号列
来源：http://hz.hywenlv.cn/gtotqdcwxa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtgrnlnsqo.html

================================================================================
来源：http://hz.shzxlz.cn/gtqcthzyhj.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtxibsklpy.html

================================================================================
来源：http://hz.redwolf501.top/gtuaatltlm.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtsefjczir.html

#!/usr/bin/env bash
来源：http://hz.xinyue.icu/gtxgzmmahp.html

set -euo pipefail
来源：http://hz.nwbrower.top/gtjewprryw.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtwrdkdicp.html

name="Tom"; echo "$name"
来源：http://hz.mhx1999.top/gtuihwotlf.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtdybycvdt.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtbwmpsikj.html

[R04] 位置参数
来源：http://hz.havefunace.top/gtoqkozgxo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtndluoron.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtmbyuvpul.html

name="${1:-default}"
来源：http://hz.chenzaomai.com/gtcauxuvtp.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtzgdtassb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yvedp.cn/gtzdofamre.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtogpcusyl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtxqukbddl.html

[R08] 数值比较
来源：http://hz.jianghu66.top/gttqdfbnbt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gturmnubpx.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtfdcryipc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtooyyyhyy.html

[R10] 正则匹配
来源：http://hz.havefunace.top/gtetasdget.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtiirfjhme.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtfgrxtgzt.html

case "$1" in
来源：http://hz.jinqigufen.top/gthlftjyut.html

start) echo "启动" ;;
来源：http://hz.pengpengdd.cyou/gtbyxrttto.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gtnboanpyf.html

*)     echo "未知命令" ;;
来源：http://hz.guannengcc.top/gtmhctkidy.html

esac
来源：http://hz.guannengcc.top/gtcudmsala.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtewsxqrfk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fengsongda.top/gtnulhirqu.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtgvngbjas.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gtjyoiyevv.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtcyhxjiwc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtgtrhmhtr.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtucezwzla.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gteordzzyz.html

[R16] until 等待条件
来源：http://hz.chenlongwang.top/gtqkcpeonl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gtnzesgval.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gttsvojdjf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtubozsoyw.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gtnnyhkudx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gaohongyu789.top/gtaioiumqg.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtiqlxxeak.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtjaxpejks.html

[R20] 关联数组（字典）
来源：http://hz.meibo888.top/gthugqqaqh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtutpurxhn.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtmvrxyqgb.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtnzgzmnhm.html

[R22] 截取子串
来源：http://hz.gzhubu.top/gthjhkcqbf.html

echo "${s:0:5}"
来源：http://hz.ppjwa.cn/gtmnncntbp.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gtwcxcpioa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gttupyefgm.html

[R24] 大小写转换
来源：http://hz.aibaodan.cn/gthzdctvqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtpkzscman.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtvbujdrmn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.daria6918.cn/gtppmohvss.html

[R26] 命令替换
来源：http://hz.hysaishi.cn/gtbezlivkz.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gthiyctvtp.html

[R27] 算术展开
来源：http://hz.gaohongyu789.top/gtmgpnvfkm.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtqukwxyeu.html

[R28] 浮点运算
来源：http://hz.gotoacloud.top/gtxoczhkya.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhaomingkeji.xyz/gtjjtuzbwt.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtrekgoxli.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gttucfitmz.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gtbsbuxalp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtwmiaathg.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtmjhzdjib.html

f() { local x=1; echo "$x"; }
来源：http://hz.ppjwa.cn/gtaijsewxk.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtxxvjapgk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.mhx1999.top/gtzmzylgao.html

[R33] 捕获错误并提示行号
来源：http://hz.iojbl.cn/gtwndhyzxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.feifeiyinyue.top/gtlwppbmau.html

[R34] 退出时清理
来源：http://hz.yangfankeji.com/gttwatwgfl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtnfgmmzmz.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangtech.top/gtjinoxbhp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtggilyest.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtuasuhvbg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtxktniwrq.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gthickcysl.html

files=$(ls -1)
来源：http://hz.xuetiantiany.cn/gtljbkutnq.html

[R38] 管道串联
来源：http://hz.zdqjudy.top/gtjayypbad.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtksvsclsb.html

[R39] 重定向标准输出与错误
来源：http://hz.yj202588.top/gtybbdguvq.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gthaadzhfu.html

[R40] 追加写日志
来源：http://hz.cdnleiting.top/gtymkjnkba.html

echo "log" >> out.log
来源：http://hz.yuxming.cn/gtnftpompy.html

[R41] 丢弃输出
来源：http://hz.sweek.top/gtxpcgtsmb.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtfszlyqve.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtlevtsqvd.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtgxkzcvsp.html

[R43] 按名字查找文件
来源：http://hz.wangshuangyany.cn/gtfrwhcpnc.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtrywgioqc.html

[R44] 按修改时间查找
来源：http://hz.52xcode.cn/gtdqcifmzh.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtcgengtci.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtdssoegok.html

find . -name "*.tmp" -delete
来源：http://hz.yongpay.top/gtwmzfwilb.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtcikvfizj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hammf.cn/gtyugxjbms.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtkxtyjdix.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj202588.top/gtzosjnnbh.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtditvuuen.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtxmuujirt.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtuvnxujwe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtkfhviojw.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtwzjvslhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtfxvcgpur.html

[R51] 排序去重取前几
来源：http://hz.tanke756.top/gtjnmwerdu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangkeji.top/gtjawwfhtf.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtowknlvys.html

wc -l a.txt
来源：http://hz.sysykeji.top/gtdxcoybbw.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtuynhpwbb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258888.top/gtgggnvekb.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtldrduxit.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtvuejsmbr.html

[R55] 压缩与解压
来源：http://hz.gzhubu.top/gtzjcneqao.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gtdsmzlhaj.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtmgqfmqik.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtvlefwwtd.html

[R57] 远程执行命令
来源：http://hz.52xcode.cn/gtlnnjyoxr.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtpyxaeflc.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtqdilvlvv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.meibo888.top/gtuipbabes.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtmqrlhbtd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtcmxnudhk.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtbmdsiygk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cheryme.top/gtzvryqcgy.html

[R61] 磁盘占用
来源：http://hz.jqgufenzy.top/gtmnqjqryg.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtlnohoyij.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gttlcgyqph.html

du -ah . | sort -rh | head -10
来源：http://hz.hongshengwenyu.top/gtiozsqrac.html

[R63] 内存与进程
来源：http://hz.yuanzhike.top/gtwodfojmc.html

free -h;  ps aux | grep nginx
来源：http://hz.shzxlz.cn/gtpwwcxvys.html

[R64] 结束进程
来源：http://hz.pengpengdd.cyou/gtdcninwdp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gttgmdbatk.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtsqdttxpe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.smart0.xyz/gtzhotwred.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtwcdvmuon.html

crontab -e;  crontab -l
来源：http://hz.jianghu66.top/gtwaacsqzj.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gtnvxtcnjf.html

openssl rand -hex 16
来源：http://hz.9152youxi.cn/gtuuouelfm.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtyfnntjus.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtavbndvif.html

[R69] 生成随机密码
来源：http://hz.hongshengwenyu.top/gtblcckblw.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtlzcwshnv.html

[R70] 时间戳与互转
来源：http://hz.mhx1999.top/gtxdmeilbt.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtbjilxixy.html

[R71] 日期格式化
来源：http://hz.guannengcc.top/gtighiaxqp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtfbyfjbph.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtvxqoffwa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ybcxt.top/gtaebucxxa.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtcybakvaj.html

split -l 1000 big.log part_
来源：http://hz.zhengqikj.top/gtgasbdzjf.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtkcssavxx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangdashe.top/gtdduswwbq.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtdtduxzut.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cdnleiting.top/gtdxzzfuzk.html

[R76] 使用临时文件
来源：http://hz.yj20258888.top/gtubccgjrw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtafojswqn.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gtkstxspds.html

read -rp "请输入: " ans
来源：http://hz.jyoumei.cn/gtnxlrpyrn.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gtkrjskjmu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yvedp.cn/gtrmhvfcts.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gttzvbfjmn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuetiantiany.cn/gtxhymqaqs.html

[R80] 查看脚本执行耗时
来源：http://hz.hnxiangtu.top/gtmwmzyqft.html

time ./run.sh
来源：http://hz.sysykeji.top/gtmrpktwlo.html

================================================================================
来源：http://hz.ydzc1.top/gtlbrspitu.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtdhylkjbi.html

================================================================================
来源：http://hz.tian-w.cn/gtpbyolfja.html

[S01] C：Hello World
来源：http://hz.sweek.top/gtjvfrhwwt.html

#include <stdio.h>
来源：http://hz.sysykeji.top/gtvuobyeai.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtdnjofxcp.html

[S02] C：变量与格式化输出
来源：http://hz.yvedp.cn/gtvnkdulgi.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtcvsokfjp.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtqdnuxunh.html

int x; scanf("%d", &x);
来源：http://hz.tian-w.cn/gtnilcdofs.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gtszawzjrg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtcvfmcrna.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtvxsegztl.html

strlen(s)
来源：http://hz.snrcjt.cn/gtgimzgprh.html

[S06] C：字符串比较
来源：http://hz.xuetiantiany.cn/gtbvzedsxm.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gthiavxeki.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtczostfcy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtpbuunakm.html

[S08] C：动态内存分配与释放
来源：http://hz.tanke756.top/gthqxtmabn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtdzyhhkvi.html

[S09] C：结构体定义与初始化
来源：http://hz.xylfe.cn/gtixsfpqqf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtnhrfekmu.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gtogocntba.html

int *p = &a;  *p = 5;
来源：http://hz.bjfxy.top/gtvztivalm.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtamxdairl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtesmpifxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258888.top/gtqiroqjze.html

fclose(f);
来源：http://hz.ydjk.org.cn/gtvvkoqzls.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtqlqmqzgh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtipjdneui.html

[S13] C：宏定义
来源：http://hz.daria6918.cn/gtuideqrtx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtoiuzmcag.html

[S14] C：枚举
来源：http://hz.aibaodan.cn/gtajyyuorz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtdiaohour.html

[S15] C：类型转换
来源：http://hz.guowangkeji.top/gtiqftkmzl.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtlpdjugkq.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtliztbtjn.html

x |= (1 << 3);
来源：http://hz.ydzc1.top/gtpgvldktm.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtgemtswbh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtygwgbdzr.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtvudseiuc.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtwmpoptzk.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gttvnojgfd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtupjkntmx.html

[S20] C：二分查找
来源：http://hz.aizwys.cn/gtpeduwrrw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtquodrkpc.html

[S21] C：字符类别判断
来源：http://hz.jqgufenzy.top/gtbpflineo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenlongwang.top/gtqkzfqcig.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gtyssultwz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtxhzuxccq.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtcexpdnqh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.feifeiyinyue.top/gtpsisybcn.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtrqbmmdjk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtemwwhcxg.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gtuwktzjzq.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtzccglzrp.html

[S26] C：内存清零
来源：http://hz.andypj.xyz/gtdliordie.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtxnbmslsw.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gttcxozjpd.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtwfalvkwx.html

[S28] C：静态变量
来源：http://hz.sufxvd.cn/gtycwwuxhd.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gtgnblrpae.html

[S29] C：变参函数
来源：http://hz.yuxming.cn/gtpakguwhw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuxming.cn/gtpwzxakrt.html

[S30] C：头文件保护
来源：http://hz.zhaomingkeji.xyz/gtyemzjlst.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtraqbvsdx.html

#define X_H
来源：http://hz.yanxiufei.cn/gtjywvmffg.html

#endif
来源：http://hz.xziqi.cn/gtedmrfkzf.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gtqhawtuxy.html

#include <iostream>
来源：http://hz.sweek.top/gtlpajltlq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hysaishi.cn/gthdgpxipz.html

[S32] C++：字符串
来源：http://hz.xuetiantiany.cn/gtsegvyrrj.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtptfsnxem.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtxgjxtvir.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtvwacznuv.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtbunbqisl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.haohaochexian.top/gtznmxgztf.html

[S35] C++：map
来源：http://hz.haohaochexian.top/gtarlatrjl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtxlydgjbs.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtvojerzbi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtelwphetu.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gtrjesdnwo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtunrcvyjw.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gthpdeimbt.html

std::sort(v.begin(), v.end());
来源：http://hz.52xcode.cn/gtizjipxag.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gtlwgeugci.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnqzz.top/gttcvxrckd.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gtjtlcfkrb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtwxbuggoa.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtcwpgbklh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gttbboazse.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtwzcxgikc.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtqlmfyotf.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtykariaey.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtfntkcndf.html

[S44] C++：引用传参
来源：http://hz.meibo888.top/gtuocgrist.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtwxvjfccc.html

[S45] C++：lambda
来源：http://hz.hnxiangtu.top/gttriwjyfe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtrctnshdj.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtsvdodykf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.svipenyu.cn/gtcslolwaj.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtzqzpetza.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtqisxtqes.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gteloowcix.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgufenzy.top/gtmokjkmzc.html

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtydadqxyb.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtmqycwgin.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtjlivzrhk.html

[S50] C++：格式化数字
来源：http://hz.nanxuanxn.top/gtginwkdat.html


<!-- 参考信息 -->
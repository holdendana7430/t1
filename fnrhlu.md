代发 wailian999

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtuzzmxuaz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtwsptscrw.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtrrqcjtmo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtimuwslbm.html

[Q80] 字符串截取
来源：http://hz.wangshuangyany.cn/gttefiasuv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenzaomai.com/gtwnijejvc.html

[Q81] 字符串替换
来源：http://hz.andypj.xyz/gtxkrzzyrd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtomhxchfx.html

[Q82] 字符长度与字节长度
来源：http://hz.snrcjt.cn/gtdrbudzya.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtknajlmfq.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gtpzfprzax.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnqzz.top/gtzowcexpw.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtasbnssyf.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtbrbwcypf.html

[Q85] 数值取整
来源：http://hz.cashguo.top/gtyktsnpwx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtbhayhdtz.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtkkaadrif.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtbeimtwnk.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtvjqpyaqz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtussofene.html

[Q88] 行转列（条件聚合）
来源：http://hz.pycfn.com/gtitsgwymb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shangyingyoupin.top/gtqrfjurag.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gthgnuvwtt.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gtpvfynhpn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtshtzdond.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtunppkqla.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnxiangtu.top/gtninscysv.html

================================================================================
来源：http://hz.hywenlv.cn/gtkurlyqlv.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtbxbbjuyd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlpipsrcu.html

[R01] shebang 与严格模式
来源：http://hz.hywenlv.cn/gtexfwggpe.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gtyopjnzgn.html

set -euo pipefail
来源：http://hz.jlsjyb.cn/gtbdkanmre.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtxftnabdl.html

name="Tom"; echo "$name"
来源：http://hz.jiagoushi.top/gtbfdunvbv.html

[R03] 只读变量
来源：http://hz.shanyushiyangtech.top/gtzeodhbtq.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtqrvzziov.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtxtxklcsa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtrbwrpdjr.html

[R05] 参数默认值
来源：http://hz.dashuyun.cn/gthliljvqv.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtgjneizdy.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtimnvrhew.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtvwdgvsqn.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gtylukceki.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hammf.cn/gtnrtjlwor.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtlnekdymy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tian-w.cn/gtlcvipurn.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtuqopmenj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtxyzmqjwj.html

[R10] 正则匹配
来源：http://hz.xinyue.icu/gtgzouboib.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhongyouzk.top/gtvkrmenov.html

[R11] case 多分支
来源：http://hz.xziqi.cn/gtayqsgrbd.html

case "$1" in
来源：http://hz.zhiwuduotai.top/gtjgyfcxrt.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtkxhwoqfr.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtzucyeike.html

*)     echo "未知命令" ;;
来源：http://hz.fengsongda.top/gtwirgirsv.html

esac
来源：http://hz.ehwqpu.com/gttqriepxc.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtfrlsrrrs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtcvcbsrge.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtimijjzal.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtyiegwydc.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtqntjvuuj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtaksxzrau.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtfykvkjpt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgfzy.top/gtxnssgdqc.html

[R16] until 等待条件
来源：http://hz.shzxlz.cn/gthktshuus.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gtazhsoctt.html

[R17] 数组定义与取值
来源：http://hz.aizwys.cn/gtkduulwnx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtwgfdpdqc.html

[R18] 遍历数组
来源：http://hz.jlsjyb.cn/gtokkgnnmi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtvsicznhp.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtfpulajmy.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtqfrrntbo.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtsghldquc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtnucshuqj.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtfmhepebo.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtsumhsxtg.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gtozgbpbnw.html

echo "${s:0:5}"
来源：http://hz.havefunace.top/gthwhrzkje.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtmmnhhrcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gteowsxcyw.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtnuepwzas.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhongyouzk.top/gtcntjnznu.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gtnppigwkh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtniczvgko.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtedrjesna.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gteuxjmqds.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtzbetqril.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtwtmzrswm.html

[R28] 浮点运算
来源：http://hz.jianghu66.top/gtcgxzlxhm.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtudqnjmmc.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtbaaglvtv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.feifeiyinyue.top/gtpqbsummw.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtkjixludv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtxfbwdprz.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gthgpaaniw.html

f() { local x=1; echo "$x"; }
来源：http://hz.gogol.net.cn/gtrrhahbvm.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtimrmsnol.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtmfvqzcdc.html

[R33] 捕获错误并提示行号
来源：http://hz.zhoulong.xyz/gtfgjgxmcy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtgvvjjaqy.html

[R34] 退出时清理
来源：http://hz.jinyuanbaomall.cn/gtfvhmrlcx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtcqdaxwdc.html

[R35] 后台执行并等待
来源：http://hz.svipenyu.cn/gtmwhzqvfj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtumvhekup.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtfefmrqxj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pycfn.com/gtpwfbiuhr.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtbvyfaght.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtrvzoesyq.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtczzjwims.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dashuyun.cn/gtptpwlbkw.html

[R39] 重定向标准输出与错误
来源：http://hz.hnqzz.top/gtanrclsby.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtvbowdbnz.html

[R40] 追加写日志
来源：http://hz.zhijiandao.cn/gteabgwcrs.html

echo "log" >> out.log
来源：http://hz.jlsjyb.cn/gtnaosneqa.html

[R41] 丢弃输出
来源：http://hz.ybcxt.top/gtpywxwcmg.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtlwjkxnno.html

[R42] 输入重定向
来源：http://hz.yuanzhike.top/gtaoiapsnl.html

wc -l < a.txt
来源：http://hz.haohaochexian.top/gtusivzvbx.html

[R43] 按名字查找文件
来源：http://hz.kuanghao11.cn/gtftejrnxt.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtnxvdekqh.html

[R44] 按修改时间查找
来源：http://hz.tianlin.xyz/gtdzctsmxt.html

find . -mtime -7 -type f
来源：http://hz.jqgfzy.top/gtsbmidnif.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtikxdcblc.html

find . -name "*.tmp" -delete
来源：http://hz.jianghu66.top/gtlqtozhbt.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtcxcoatzn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj202588.top/gtsmpzrezl.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtfvcktxun.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnqzz.top/gtgkduzoob.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtxdepkawx.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtllnlywxz.html

[R49] awk 带条件
来源：http://hz.sweek.top/gtnxmtsexe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gthsmklfhg.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtisybijgb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yongpay.top/gtxibhpajb.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtwyuvlhoc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtsrvcfbsi.html

[R52] 统计行数
来源：http://hz.hysaishi.cn/gtrcilzieb.html

wc -l a.txt
来源：http://hz.zhiwuduotai.top/gtdagnrlrb.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtweprkrqr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtpimvsmco.html

[R54] 比较两个文件
来源：http://hz.hongshengwenyu.top/gtxclxlhvw.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtdwqatytl.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtrzpsvvvk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.birdmap.top/gtzgeotcqj.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtnqhhjpmn.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtpfeolnww.html

[R57] 远程执行命令
来源：http://hz.gotoacloud.top/gthcbovbsf.html

ssh user@host 'uptime'
来源：http://hz.hysaishi.cn/gtonsxkjgh.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtqoepteko.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zycfv.cn/gtskvjbxom.html

[R59] 发 POST JSON
来源：http://hz.shzxlz.cn/gtoouqlort.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtzfkogrha.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gttylbtltt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtaihxofyn.html

[R61] 磁盘占用
来源：http://hz.kuanghao11.cn/gtiztczfbd.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtvlcsuyqc.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtxqgymzhh.html

du -ah . | sort -rh | head -10
来源：http://hz.hammf.cn/gtjnzjzryd.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtcdwxlzbj.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtpisnnakt.html

[R64] 结束进程
来源：http://hz.nanxinkj.top/gtbxchtkog.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtfelvzdzl.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtwszosufr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtanwonarg.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gtyihxhovc.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtwpaqoxbs.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtexytsqcs.html

openssl rand -hex 16
来源：http://hz.c1oappe.top/gtboidbjvc.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtgazvrwmp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtnsyedmgz.html

[R69] 生成随机密码
来源：http://hz.jqgufenzy.top/gtuspkrvjw.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtkwixgihf.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtrgqljiyw.html

date +%s;  date -d @1700000000
来源：http://hz.guannengcc.top/gtultpfofp.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtqpdadtsy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtyvfklkqc.html

[R72] 等待端口就绪
来源：http://hz.sysykeji.top/gtuparoapy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtxqltkcos.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gtmqcidqqm.html

split -l 1000 big.log part_
来源：http://hz.316326.xyz/gtgjempyvx.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtlfzoewfr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtsbbmvyfc.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtbreqkpqg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinyuanbaomall.cn/gtmouxwdut.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtrpuacqyv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtfmujmyju.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gteqpfvkyc.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtujikumuc.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtgunbsjgf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gthxqcvwne.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtugnihowe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtpwwptmpk.html

[R80] 查看脚本执行耗时
来源：http://hz.shzxlz.cn/gtuxzsnxdb.html

time ./run.sh
来源：http://hz.smart0.xyz/gturyxdtzw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtsvmesnlo.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtdrdmupbe.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtuvgqgzds.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtihhigobn.html

#include <stdio.h>
来源：http://hz.yonumen.top/gttjihwlrb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtirguoniz.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gtxvmooyrq.html

int a = 10; printf("%d\n", a);
来源：http://hz.guannengcc.top/gtabqslnbb.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtbmppuvxb.html

int x; scanf("%d", &x);
来源：http://hz.9152youxi.cn/gtrxncsido.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtcpxhbnfd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhaomingkeji.xyz/gthkkfinei.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gtkhseriuk.html

strlen(s)
来源：http://hz.yj20258888.top/gtwrcdcwjk.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtfasqzdpp.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtkfoldlsd.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtpllrsyqg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtpiocccfo.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtqhnrhfml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtnerlsisw.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gtftofosoy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sufxvd.cn/gtbvbjwala.html

[S10] C：指针与解引用
来源：http://hz.jqgfzy.top/gtnyghtmso.html

int *p = &a;  *p = 5;
来源：http://hz.nanxinkj.top/gtvswaczav.html

[S11] C：逐行读文件
来源：http://hz.zhoulong.xyz/gtixzoooba.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gtcedmtbps.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gttkkxrhen.html

fclose(f);
来源：http://hz.nanxuanxn.top/gthcqtufpa.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtgjofgnnu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gttzhzakeo.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtohdxgvwh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuetiantiany.cn/gtkqyvzbcg.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtvjngtecb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtjegdrpag.html

[S15] C：类型转换
来源：http://hz.yuanzhike.top/gtpgmolzsp.html

(double) a / b
来源：http://hz.shuidangran.top/gtgubmabhc.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtcempdxfn.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtcbsjkgqa.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gthqontufx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtyprvjgyi.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtikquyazi.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtyjhufkxc.html

[S19] C：快速排序
来源：http://hz.birdmap.top/gtqrfyhvsj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtsjpzeacv.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gtyedwsqun.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtegkhoadv.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtzccnsjbj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhengqikj.top/gtsejaquuw.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gtcmmqpwvq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gternljumj.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtspsblgvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hongshengwenyu.top/gtyxappkpr.html

[S24] C：获取本地时间
来源：http://hz.meibo888.top/gtexrmryhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtoddanjlm.html

[S25] C：内存拷贝
来源：http://hz.dianchejie.cn/gtimaoeudz.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtzegkrzyx.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtoclhmkrb.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtpucqmlxt.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gtmksjctrb.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtconrnfgb.html

[S28] C：静态变量
来源：http://hz.jlsjyb.cn/gtenumdrwn.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtxiojjsic.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtdgskolrc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtndcwwcti.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtqekczmoo.html

#ifndef X_H
来源：http://hz.ehwqpu.com/gtpkzmwdfx.html

#define X_H
来源：http://hz.ydjk.org.cn/gtlbnzzjcn.html

#endif
来源：http://hz.ehwqpu.com/gtuqvifetb.html

[S31] C++：Hello World
来源：http://hz.jqgufenzy.top/gtizymaxxu.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtnlwtbbnw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guannengcc.top/gtbotwlgip.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtamcjeyvj.html

std::string s = "hi";  s += "!";
来源：http://hz.yonumen.top/gtiyxwutaw.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtwiqemgle.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtynheuuug.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtkkerkkna.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guowangkeji.top/gtrnncfjhn.html

[S35] C++：map
来源：http://hz.gaohongyu789.top/gtqkogvgbz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtkkadprdr.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gteitzsjyk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtdptzmtfy.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtbdgahlcl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dashuyun.cn/gtxhfzikng.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtzkubmmww.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtoetdztma.html

[S39] C++：自定义比较器排序
来源：http://hz.wangshuangyany.cn/gtofwhpqng.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daxiang520.top/gtnlesczfo.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtwrfadlxy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtyanjszyu.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtrdfueypx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtnukstlzk.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtfpgurjdd.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtvhzphlaj.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gturjmaxni.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtzsplskxq.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtjzjoalxp.html

void inc(int &x) { ++x; }
来源：http://hz.xziqi.cn/gtpfbzagwk.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtcnrdncio.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtjwqextlm.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gthireyvbc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dianchejie.cn/gtjkwaekgu.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gtedwxvihe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gttzcbnqwy.html

[S48] C++：逐行读文件
来源：http://hz.0kj1m.cn/gtzxmijjag.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtletydofq.html


<!-- 参考信息 -->
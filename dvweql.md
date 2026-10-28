代发 wailian999

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gthprsfhgg.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtlvkjqhtc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtsufuubbx.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtxhtkckvg.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtypstvcxs.html

[Q73] 查看表状态
来源：http://hz.andypj.xyz/gtbvpsbvnw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gtxxdmqxrj.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtnyfniptx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jiagoushi.top/gtjauvfulx.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtqrgomrqq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258.top/gtveobcxjq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtumfdffdn.html

[Q76] 按天统计
来源：http://hz.shanyushiyangkeji.top/gtfddtiihk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gtgxkjouhw.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtlbdrylpg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.0kj1m.cn/gtckhbexbd.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtoaulmmkj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shzxlz.cn/gtbexxrlin.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtxdtcjuok.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sweek.top/gtmzgedzru.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtdntscwwz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtoybldftn.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtxdlqnqeu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtvimufztk.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gtktwuqhzo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtbkaidlpf.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtcsnnbaoq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hammf.cn/gttpmyqzsr.html

[Q84] 去除首尾空格
来源：http://hz.vqdsnc.cn/gtbzcljqgl.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenlongwang.top/gtusougfqs.html

[Q85] 数值取整
来源：http://hz.yuanzhike.top/gtyymvjowx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuanzhike.top/gtuvlyfmll.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtiuiibfwb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtwewcwmta.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gtuhfltkwo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gtxpkfvqjh.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtderfirxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gtbkrrhaua.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtbhzbyimi.html

[Q89] 判断表是否存在
来源：http://hz.jqgfzy.top/gttwegerso.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtwntohfpr.html

[Q90] 生成序号列
来源：http://hz.9152youxi.cn/gtplwnycrw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daxiang520.top/gtlllysmyw.html

================================================================================
来源：http://hz.daxiang520.top/gtevviljcq.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtwduvpysw.html

================================================================================
来源：http://hz.fengsongda.top/gtefsnqcli.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtoqowojre.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtcvggfrzx.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtjcvbknqq.html

[R02] 变量赋值与使用
来源：http://hz.hnxiangtu.top/gtrnntcwdv.html

name="Tom"; echo "$name"
来源：http://hz.smart0.xyz/gtxfkzxkax.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtbvdjyssy.html

readonly PI=3.14
来源：http://hz.gaohongyu789.top/gtfonenmbl.html

[R04] 位置参数
来源：http://hz.nanxuanxn.top/gttysancca.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtemshejnn.html

[R05] 参数默认值
来源：http://hz.cheryme.top/gtvjhmsmai.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtkxgpaqme.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtaenluats.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gthkemcqqj.html

[R07] if 判断文件
来源：http://hz.52xcode.cn/gtivekvdcm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtedpnwwvx.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtplqwgyoa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtwvwlpivi.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtjdkqzraf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtctsdpbiu.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtqiwtmais.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sxryk.cn/gtxwlqioxy.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gthvkfpomq.html

case "$1" in
来源：http://hz.haohaochexian.top/gtbarfougi.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gthalyipef.html

stop)  echo "停止" ;;
来源：http://hz.gotoacloud.top/gtolnuwelg.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtqhgmceae.html

esac
来源：http://hz.haohaochexian.top/gtrsqicgpv.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtnwvbtdmm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtwibjsnee.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gttoppfjaz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gthlbqunwm.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtbmshizwo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtirlgndai.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtddyzvchu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtxyfndcyt.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtwdlczwnc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtnsbfmpue.html

[R17] 数组定义与取值
来源：http://hz.cheryme.top/gtojdgnlrs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtmluipwxf.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gteoshnixk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtkxmigbos.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtwnjfcjua.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtvjnxlbyt.html

[R20] 关联数组（字典）
来源：http://hz.cashguo.top/gtozkmdozq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtrjhwgiyl.html

[R21] 字符串长度
来源：http://hz.smart0.xyz/gtyzbtjtvy.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gteqvyqluk.html

[R22] 截取子串
来源：http://hz.yuxming.cn/gtlmhbvaax.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtqoqynvqd.html

[R23] 字符串替换
来源：http://hz.hammf.cn/gthlrpigso.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daxiang520.top/gtzazpndus.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtyvunsfvs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtygrotmcq.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtelxcxnmj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtgrrmkqhx.html

[R26] 命令替换
来源：http://hz.yongpay.top/gtsfjdncgp.html

now=$(date +%F); echo "$now"
来源：http://hz.aizwys.cn/gtrbffmvxt.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtrgbiekzt.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtkqnujktd.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtzkphisvv.html

echo "scale=2; 10/3" | bc
来源：http://hz.guowangkeji.top/gtyqyzrpyy.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtzjoxvvhf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gthrgelkwt.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtbgwraery.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.quarkkingdee.top/gtexvsbisv.html

[R31] 局部变量
来源：http://hz.zhijiandao.cn/gtydhjmmkz.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gttfvicigk.html

[R32] 参数个数校验
来源：http://hz.gzhubu.top/gtjzrocaog.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtgdntfiyf.html

[R33] 捕获错误并提示行号
来源：http://hz.sysykeji.top/gtgvlugrdo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtblxgeleq.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtwjojqppr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtcmotguwr.html

[R35] 后台执行并等待
来源：http://hz.zhaomingkeji.xyz/gtkmkiwplw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ivvv.top/gthcfmuzsx.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtjptzsuha.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtryqxyaab.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtscwoxeec.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtxketomft.html

[R38] 管道串联
来源：http://hz.xylfe.cn/gtqebkqafj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtpfmnplyy.html

[R39] 重定向标准输出与错误
来源：http://hz.fzhhl.top/gtrthqbdsy.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtuzutfuro.html

[R40] 追加写日志
来源：http://hz.nanxinkj.top/gtzxltrgrg.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtyvcratyk.html

[R41] 丢弃输出
来源：http://hz.yj202588.top/gtfqpdqqnj.html

cmd >/dev/null 2>&1
来源：http://hz.zhengqikj.top/gtscbirhfz.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtrkilvmcm.html

wc -l < a.txt
来源：http://hz.xziqi.cn/gtlsqjumih.html

[R43] 按名字查找文件
来源：http://hz.ivvv.top/gtfvvgjxks.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gttdqtelsd.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtaguugwzt.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtwwimxzgw.html

[R45] 批量删除
来源：http://hz.chenjidiqi.icu/gthreslgcl.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtcvwzxtum.html

[R46] 递归替换文件内容
来源：http://hz.hywenlv.cn/gtieyettvr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yongpay.top/gtsfgpntdq.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtvdehehkf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gaohongyu789.top/gtpqqwdirp.html

[R48] awk 取指定列
来源：http://hz.yonumen.top/gtyywhwnim.html

awk '{print $1, $3}' a.txt
来源：http://hz.guowangkeji.top/gtcuplxqas.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtjnolifwu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtfgtsueqo.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtshbgmawu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtccjjmhqa.html

[R51] 排序去重取前几
来源：http://hz.hnqzz.top/gtfzmcrryv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtjttjhulx.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtmzizfegs.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtbskbdgei.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtocjsupuj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gthakuudqp.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtbqttmzfn.html

diff a.txt b.txt
来源：http://hz.jianghu66.top/gtimgyclkq.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtbvgcbzdh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gtthbyvbsi.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtmztqkhbl.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gtmrrmhfwv.html

[R57] 远程执行命令
来源：http://hz.daxiang520.top/gttimvkcge.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtisahnkdc.html

[R58] 下载文件
来源：http://hz.ehwqpu.com/gtbtvlbiwu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtdiajdiqr.html

[R59] 发 POST JSON
来源：http://hz.cheryme.top/gttcyaeijj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenjidiqi.icu/gtnlhkqjkh.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtjzyhqlvx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.havefunace.top/gtcyxbtrsx.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gtmnefepdx.html

df -h;  du -sh *
来源：http://hz.svipenyu.cn/gtzrnlrcrf.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gtvfbhpdsv.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gtkvunbksd.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtgjlmigqn.html

free -h;  ps aux | grep nginx
来源：http://hz.guannengcc.top/gtzzmeadic.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtjusaukpy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtormuhpvj.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtrkzsicog.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtutfbuwci.html

[R66] 定时任务
来源：http://hz.yueranfly.top/gttzkevqnf.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtppzuzzbl.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gtbnztuamk.html

openssl rand -hex 16
来源：http://hz.jianghu66.top/gtwfrjtkbu.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtzzbqkqjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuanzhike.top/gtqmanlzul.html

[R69] 生成随机密码
来源：http://hz.kuanghao11.cn/gtgaoydvaz.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtehbhwoub.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtgevidtxu.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gteodphdmg.html

[R71] 日期格式化
来源：http://hz.shzxlz.cn/gtsptepwye.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gzhubu.top/gtutzkdhwc.html

[R72] 等待端口就绪
来源：http://hz.jinqigufen.top/gtghodrhzr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtiguozoac.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtpmxtvgnf.html

split -l 1000 big.log part_
来源：http://hz.hnxiangtu.top/gtovjiowrv.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtuelpbhfh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtulriairx.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtiofcqxhh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.meibo888.top/gtwugzsldp.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtuknqeyev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gthjkggxpy.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtcbpddfml.html

read -rp "请输入: " ans
来源：http://hz.xylfe.cn/gtktohikjp.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtnulhuncl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtkhttllyg.html

[R79] 解析命令行选项
来源：http://hz.yvedp.cn/gtryoytjpr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gaohongyu789.top/gtgtbldzbc.html

[R80] 查看脚本执行耗时
来源：http://hz.xingfuxueyuan.xyz/gttqlmwcxc.html

time ./run.sh
来源：http://hz.bjfxy.top/gtwkmiclye.html

================================================================================
来源：http://hz.ydzc1.top/gtvxlbzyfo.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gtrbgvkdhk.html

================================================================================
来源：http://hz.zycfv.cn/gtiaiuysai.html

[S01] C：Hello World
来源：http://hz.zhongyouzk.top/gtadnnastu.html

#include <stdio.h>
来源：http://hz.sysykeji.top/gtkrghcowj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gthhulfmoz.html

[S02] C：变量与格式化输出
来源：http://hz.jinghuilouyu.cn/gtsefkciem.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gtxdczugzi.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtbwajffpn.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtndnjddnl.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtjfegkfwa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtghxmxsjc.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtvsflswqo.html

strlen(s)
来源：http://hz.jyoumei.cn/gtnuvclrwu.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gttrubvwal.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtzepnggsv.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtryfyidfd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtbrnnfdpf.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtumqkockp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhongyouzk.top/gtdlwpubjo.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gteupbeohv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtohlcknov.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtjfasooqv.html

int *p = &a;  *p = 5;
来源：http://hz.jianghu66.top/gtnlwyenws.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtrpqgcguj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtradywtsa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtdbgebafw.html

fclose(f);
来源：http://hz.zycfv.cn/gtmacjjhsw.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtttgfhzzh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtzmlkdnip.html

[S13] C：宏定义
来源：http://hz.gaohongyu789.top/gtxrfeyalr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtusxeealu.html

[S14] C：枚举
来源：http://hz.zycfv.cn/gtislxqmbk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtjckigocj.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtizaobpat.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtirmfzqgv.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtuuksvvny.html

x |= (1 << 3);
来源：http://hz.yj20258.top/gtlkvgrwlq.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gthshrtbjo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhixingplan.top/gtsaslkvvb.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtwirflfnw.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtbazxmimj.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtxvaoovgk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtkbkrkfvs.html

[S20] C：二分查找
来源：http://hz.cashguo.top/gtznicnfhh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtespdsyfd.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtcekedglv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258888.top/gtzexttlhl.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gteppqtlil.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtuutppbls.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtgdgyipin.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtpuzpahcq.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtbiujsnlv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nwbrower.top/gtzzvjfqgi.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtjwlpbffp.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gthfxgadvx.html

[S26] C：内存清零
来源：http://hz.xinyue.icu/gtgseatoqn.html

memset(a, 0, sizeof a);
来源：http://hz.cheryme.top/gtauqidyvb.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtspfjcbfg.html

const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtwwkhyhum.html

[S28] C：静态变量
来源：http://hz.nanxinkj.top/gthghhrvum.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtegjbbcgj.html

[S29] C：变参函数
来源：http://hz.yvedp.cn/gtoaebnnky.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangdashe.top/gtsszvbfww.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gtdiuvrfjt.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtqubsxvyz.html

#define X_H
来源：http://hz.bjfxy.top/gtizhshhxu.html

#endif
来源：http://hz.sufxvd.cn/gtwtdjedog.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gtztnjkfll.html

#include <iostream>
来源：http://hz.ybcxt.top/gtrkvdeing.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtbesnfzcd.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gteuyzeqpy.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtnvqtqcjs.html

[S33] C++：vector 增删
来源：http://hz.52xcode.cn/gtvjkeqoyq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtbgjoemml.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gtutxmykfl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sweek.top/gtufdzpbfz.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gtpqhctkhi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtikzaqput.html

[S36] C++：unordered_map
来源：http://hz.hongshengwenyu.top/gtnxjtiacw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtruvpdzag.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtmmpiawdn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhixingplan.top/gtntvaegat.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtgzsopqkc.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtkbnnjrqi.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtyisjelgi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtxydchwfp.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtwrhdelte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gteizvdbdt.html


<!-- 参考信息 -->
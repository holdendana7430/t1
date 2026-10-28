代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.bjfxy.top/gtjpwvcbjo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gtozxbvdip.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gtlysbqovy.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gtpiwrfiiy.html

ROLLBACK TO sp1;
来源：http://hz.cdnleiting.top/gtcllnqwij.html

[Q69] 查看执行计划
来源：http://hz.c1oappe.top/gtiesimlyw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.bjfxy.top/gtazxmaavn.html

[Q70] 更新统计信息
来源：http://hz.tianlin.xyz/gtrxgtuvnp.html

ANALYZE TABLE users;
来源：http://hz.yj20258.top/gtbdajzwsl.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtqzqkxcrv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.iojbl.cn/gthrxmumfc.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtpmylcwiw.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gtltnysztg.html

[Q73] 查看表状态
来源：http://hz.0kj1m.cn/gteeosccnn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shuidangran.top/gtjvngyqxn.html

[Q74] 强制使用索引
来源：http://hz.sufxvd.cn/gtkfgzuhqa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ehwqpu.com/gtajxwoxlz.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtufxrfbgc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtlojqxutq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hywenlv.cn/gtfwvkfgpy.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gttpbzdonr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxinkj.top/gtjsrnsksn.html

[Q77] 时间加减
来源：http://hz.52xcode.cn/gtedldlxjl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gtluawgayo.html

[Q78] 当前时间
来源：http://hz.xuanzx.com/gtakatcszp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gtyoiexjvw.html

[Q79] 字符串拼接
来源：http://hz.pycfn.com/gtjxllnqbl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtzvhqvnyh.html

[Q80] 字符串截取
来源：http://hz.tian-w.cn/gtbqvxbdmu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenzaomai.com/gtzuetukcw.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtdrstvzef.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.iojbl.cn/gtfxijppkn.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtxqtqrbsc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtjhxgeeak.html

[Q83] 大小写转换
来源：http://hz.ydjk.org.cn/gtmftwjmzz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.0kj1m.cn/gtxpubtelq.html

[Q84] 去除首尾空格
来源：http://hz.wangdashe.top/gtixzzgmmy.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydzc1.top/gtqgjhynan.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtchxkzqyg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtynjatevu.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gthkytooiq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtugwqngsg.html

[Q87] JSON 字段做条件
来源：http://hz.fzhhl.top/gtldhfdxhs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtabezvpst.html

[Q88] 行转列（条件聚合）
来源：http://hz.316326.xyz/gticlwwogz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.kuanghao11.cn/gtfxtdrvve.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zdqjudy.top/gtlgajmosi.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtpwkkgakx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sysykeji.top/gttcvvxwbx.html

[Q90] 生成序号列
来源：http://hz.hysaishi.cn/gtvnbfuqjj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtietmscgc.html

================================================================================
来源：http://hz.yongpay.top/gtidpdwvzr.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtvjawmeyf.html

================================================================================
来源：http://hz.daxiang520.top/gtlyehfzds.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gticxrmucr.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gthpnlzxhz.html

set -euo pipefail
来源：http://hz.ppjwa.cn/gtonsxylwd.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gtnijbiuhk.html

name="Tom"; echo "$name"
来源：http://hz.havefunace.top/gtnujchibm.html

[R03] 只读变量
来源：http://hz.redwolf501.top/gtxzsselac.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtkvnmeryy.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtnnzjrdig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hfpthk.cn/gteqkmwbzo.html

[R05] 参数默认值
来源：http://hz.yj20258.top/gtfzmqnshw.html

name="${1:-default}"
来源：http://hz.chenjidiqi.icu/gthpbvfcze.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtgsuiepep.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xylfe.cn/gtphqsyajc.html

[R07] if 判断文件
来源：http://hz.tian-w.cn/gtdzkhxukh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.feifeiyinyue.top/gtmxhqzkwk.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtfkmwxgqu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtmtlltqxc.html

[R09] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtcfgpvfmb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtdmizsziw.html

[R10] 正则匹配
来源：http://hz.guowangkeji.top/gtqydjdxsv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.mhx1999.top/gtznzekusw.html

[R11] case 多分支
来源：http://hz.ivvv.top/gtzgbjtsiu.html

case "$1" in
来源：http://hz.c1oappe.top/gtctspzsfx.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtidziidug.html

stop)  echo "停止" ;;
来源：http://hz.jinghuilouyu.cn/gtcmcluwhq.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtmuwcfwoi.html

esac
来源：http://hz.daxiang520.top/gtdlmelpfu.html

[R12] for 遍历文件
来源：http://hz.cashguo.top/gtiviljenm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gaohongyu789.top/gtemlgkevj.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtbdcgscqv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gttxytdjbx.html

[R14] C 风格 for
来源：http://hz.cqqwz.cn/gtnuybijxd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gthriklfwh.html

[R15] while 逐行读文件
来源：http://hz.tian-w.cn/gtlbiywfnp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtaoshabom.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtomdbvykr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gthsxhzsxe.html

[R17] 数组定义与取值
来源：http://hz.nanxinkj.top/gtkeyjfkhf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtvtdmqjzp.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtxnyheiug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtpprexukv.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtqttdkrxc.html

echo "${#arr[@]}"
来源：http://hz.pycfn.com/gtikkzhfdp.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtexgvnugu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.kuanghao11.cn/gtasmkxewj.html

[R21] 字符串长度
来源：http://hz.cqqwz.cn/gtidcojrzb.html

echo "${#s}"
来源：http://hz.cqqwz.cn/gtznfcphys.html

[R22] 截取子串
来源：http://hz.tanke756.top/gtuvayrzvs.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangtech.top/gtexgnyqzz.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gthdulspkw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yanxiufei.cn/gtjnmvohyv.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtgfwtlxyi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gttbcfnfnm.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtsaweinda.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtkeancwdh.html

[R26] 命令替换
来源：http://hz.jqgfzy.top/gttgjbefts.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtsbvaawrt.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtsrirareq.html

echo $((1 + 2 * 3))
来源：http://hz.hywenlv.cn/gttsdypheh.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gthdwdiyjd.html

echo "scale=2; 10/3" | bc
来源：http://hz.shzxlz.cn/gtjkiaeubz.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtroxaosud.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhijiandao.cn/gtgldmizxq.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtgvxutzee.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.52xcode.cn/gtckupibdj.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gtgvpktzgk.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gtbfyzynal.html

[R32] 参数个数校验
来源：http://hz.snrcjt.cn/gtmxakzvtp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.meibo888.top/gtzablkfdg.html

[R33] 捕获错误并提示行号
来源：http://hz.chenzaomai.com/gtvctdorwb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cdnleiting.top/gtddntdbqn.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtgyeegndj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtgarcxoou.html

[R35] 后台执行并等待
来源：http://hz.jinqigufen.top/gtjpjkrwny.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtqithuasi.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtylrelwti.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtohhucsof.html

[R37] 把输出赋给变量
来源：http://hz.gzhubu.top/gtgcttpdml.html

files=$(ls -1)
来源：http://hz.dianchejie.cn/gtskfyameb.html

[R38] 管道串联
来源：http://hz.kuanghao11.cn/gtpaotxsrm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtkndcjdya.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gtqsotbwyh.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gttharuotb.html

[R40] 追加写日志
来源：http://hz.redwolf501.top/gtqnrflwgi.html

echo "log" >> out.log
来源：http://hz.jinqigfzy.top/gtahfoevci.html

[R41] 丢弃输出
来源：http://hz.ivvv.top/gtrszhbylw.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtewkmcnwi.html

[R42] 输入重定向
来源：http://hz.gzhubu.top/gtwmxbfrfz.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtexwajafr.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gtsxeojdjd.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangtech.top/gttspnmqob.html

[R44] 按修改时间查找
来源：http://hz.zhengqikj.top/gttsuiepbl.html

find . -mtime -7 -type f
来源：http://hz.svipenyu.cn/gteijtlbjq.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtzbzahksf.html

find . -name "*.tmp" -delete
来源：http://hz.zhongyouzk.top/gtrxwzzvlb.html

[R46] 递归替换文件内容
来源：http://hz.0kj1m.cn/gtbrrdccmd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jianghu66.top/gttieiiuyo.html

[R47] sed 单行替换
来源：http://hz.svipenyu.cn/gtalmkqzvu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gtcnlbarba.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gtmnjoqfym.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtpewzfqmm.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtvlietnzd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtymfyyytt.html

[R50] awk 求和
来源：http://hz.zhoulong.xyz/gtiiuztuzo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuxming.cn/gttdbyehnr.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtlgrqmcym.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.smart0.xyz/gtilqrbhvv.html

[R52] 统计行数
来源：http://hz.jinqigfzy.top/gtmyeneegg.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gtxpdfeyrt.html

[R53] 查看文件头与实时尾
来源：http://hz.c1oappe.top/gtbdcuczof.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yueranfly.top/gtlgbnrgfh.html

[R54] 比较两个文件
来源：http://hz.dianchejie.cn/gtiuqycsmu.html

diff a.txt b.txt
来源：http://hz.bjfxy.top/gtqcdjgzlr.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtqjeckoho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guannengcc.top/gtvjkhzyjv.html

[R56] 远程拷贝
来源：http://hz.zhongyouzk.top/gtcpsjkhyd.html

scp file user@host:/path/
来源：http://hz.nanxinkj.top/gtplcaomve.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtcazqarrp.html

ssh user@host 'uptime'
来源：http://hz.havefunace.top/gtguumfyzk.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gthrqcxunt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtmlfzekxe.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gthzgkbxub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtdeghhytt.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtrqbefrxh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zdqjudy.top/gtwytqpusb.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtsbazkecw.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gtdrwihjkx.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtdtngdmqx.html

du -ah . | sort -rh | head -10
来源：http://hz.andypj.xyz/gtjwldnbfw.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtifcydtuc.html

free -h;  ps aux | grep nginx
来源：http://hz.hnxiangtu.top/gtviwnufxm.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtsavcuzgc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtcmcbitzt.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtohwfwomz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtdcmnumfa.html

[R66] 定时任务
来源：http://hz.gotoacloud.top/gtlywrkdae.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtvaippfrh.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gtlecpyuyj.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtthddlpiy.html

[R68] 计算文件校验值
来源：http://hz.cheryme.top/gtqihdmmnq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtjmxgoksi.html

[R69] 生成随机密码
来源：http://hz.tianlin.xyz/gtdsuzzmkj.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtrurrbhec.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtqgkcxgvi.html

date +%s;  date -d @1700000000
来源：http://hz.sweek.top/gtptmzsksk.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gtsufsrwsm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtqbxgskij.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtysossnhu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gtpizfqklm.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gtvfveifzx.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtomekruzw.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gteansvnum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtgcznusrl.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gttyaxaqlr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtnbqytuee.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtgaqlqbmd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtjeazugjc.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtggnofmhq.html

read -rp "请输入: " ans
来源：http://hz.daria6918.cn/gtetdjxcnb.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtwqewgcqp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gthxytxsee.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtykxrrhzs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cashguo.top/gtqawkypxa.html

[R80] 查看脚本执行耗时
来源：http://hz.yuanzhike.top/gttzwggerv.html

time ./run.sh
来源：http://hz.sysykeji.top/gtghgmdlyg.html

================================================================================
来源：http://hz.52xcode.cn/gtbkkfnaro.html

S. C / C++ 专题
来源：http://hz.gogol.net.cn/gtozgfqtwb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzhbqgcdk.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtmsdmpmvh.html

#include <stdio.h>
来源：http://hz.yangfankeji.com/gtfeocvqcg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtufkdahtl.html

[S02] C：变量与格式化输出
来源：http://hz.hammf.cn/gtonwecfqb.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtuxjcoytf.html

[S03] C：读入整数
来源：http://hz.yuxming.cn/gtcguazhnm.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtoizdfqwr.html

[S04] C：字符串复制
来源：http://hz.guannengcc.top/gteuyncmwa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtvqaqfdvf.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtozmuskac.html

strlen(s)
来源：http://hz.0kj1m.cn/gtbksoiaiu.html

[S06] C：字符串比较
来源：http://hz.kuanghao11.cn/gtmnkncbpe.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gttbyogzpj.html

[S07] C：数组遍历求和
来源：http://hz.hnqzz.top/gtmrivwonn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.andypj.xyz/gtouzvidbh.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gtgcrwxhjr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aibaodan.cn/gtqdlnhdlz.html

[S09] C：结构体定义与初始化
来源：http://hz.hammf.cn/gthupmstmf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtwaktvngg.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtdzaozlnr.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtxgesrpna.html

[S11] C：逐行读文件
来源：http://hz.jqgufenzy.top/gthzpuklao.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtnqhdwbsq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtjgtyqeru.html

fclose(f);
来源：http://hz.shuidangran.top/gtengkjyej.html

[S12] C：写文件
来源：http://hz.fzhhl.top/gtuqbnulrj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtjxvurnue.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtxksuilyf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gtwrgefgmy.html

[S14] C：枚举
来源：http://hz.birdmap.top/gthkipjhmi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shuidangran.top/gtbidrymoj.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtuqlkfprs.html

(double) a / b
来源：http://hz.9152youxi.cn/gtwrfhsydj.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtgavqntcc.html

x |= (1 << 3);
来源：http://hz.tianlin.xyz/gtafnqbxry.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtdpqfaxza.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aibaodan.cn/gtjxhgjlru.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtugvptaen.html

int main(int argc, char **argv)
来源：http://hz.haohaochexian.top/gtagwynyma.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtvcaciuvg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtqhpsndgc.html

[S20] C：二分查找
来源：http://hz.zhixingplan.top/gtghqdbdva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtnvkiiqdl.html

[S21] C：字符类别判断
来源：http://hz.yongpay.top/gtjrvqzbej.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhaomingkeji.xyz/gtkoxxjcgq.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtejdyahpi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shzxlz.cn/gtftnmpxcu.html

[S23] C：随机数
来源：http://hz.shuidangran.top/gtuirgrqgx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtabeqtovo.html

[S24] C：获取本地时间
来源：http://hz.jinqigufen.top/gtylkbfiay.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.haohaochexian.top/gtbyvqkreh.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtysdrpvri.html

memcpy(dst, src, n);
来源：http://hz.316326.xyz/gthvymmild.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtxnqdvzgd.html

memset(a, 0, sizeof a);
来源：http://hz.zhaomingkeji.xyz/gtnwhbbcmg.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gtzfthpnar.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gthrseuqos.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtuowngqam.html

static int counter = 0;
来源：http://hz.52xcode.cn/gtjucdpuev.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtykgnglec.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtezbmavwi.html

[S30] C：头文件保护
来源：http://hz.smart0.xyz/gthphimqom.html

#ifndef X_H
来源：http://hz.yongpay.top/gtgqwjhtez.html

#define X_H
来源：http://hz.iojbl.cn/gtguvawqcz.html

#endif
来源：http://hz.zdqjudy.top/gtyhfaxcdn.html

[S31] C++：Hello World
来源：http://hz.wangdashe.top/gtgjmkabpk.html

#include <iostream>
来源：http://hz.zhijiandao.cn/gthdmgupwc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sweek.top/gtlywanqxp.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gttzoagijr.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtjtbyowpm.html

[S33] C++：vector 增删
来源：http://hz.jqgufenzy.top/gtmxtenzpn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtzsseefvf.html

[S34] C++：遍历 vector
来源：http://hz.tanke756.top/gtqrsvzgci.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gtemxakaul.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gtexacaxlz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtnljcbcxw.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtuypydplz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtahirfoyr.html


<!-- 参考信息 -->
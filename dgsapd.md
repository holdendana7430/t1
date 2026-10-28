代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtnniajnwt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtklelofos.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gtyrvgpdts.html

[Q57] 行号
来源：http://hz.yj20258.top/gtvazepado.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jianghu66.top/gtvfzvkhiq.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtpmcjwczk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hongshengwenyu.top/gtvilqksrw.html

[Q59] 分组内累计
来源：http://hz.zycfv.cn/gtntmgtbgt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yuanzhike.top/gtkzmttyod.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtbtomffsv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gtsefnhrun.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gtwuwrsjqj.html

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtzgdlfptl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hongshengwenyu.top/gtvffxgcxp.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtowmutpqi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtralhwsfs.html

[Q63] 开启事务
来源：http://hz.andypj.xyz/gtnrdjopct.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aibaodan.cn/gtlilcutvb.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtxyitoaui.html

COMMIT;
来源：http://hz.shangyingyoupin.top/gtspdplvkx.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtfqplzxwo.html

ROLLBACK;
来源：http://hz.cashguo.top/gtffkhsdgq.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtpfryjnit.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgufenzy.top/gtidnmmujx.html

[Q67] 设置隔离级别
来源：http://hz.gzhubu.top/gteejmtcsw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gtvmrrccds.html

[Q68] 保存点
来源：http://hz.fzhhl.top/gtitdxskbg.html

SAVEPOINT sp1;
来源：http://hz.ydjk.org.cn/gtgbgzfuem.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtnoxjfaah.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gtmdgjmqyt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gtoosmpcrx.html

[Q70] 更新统计信息
来源：http://hz.316326.xyz/gtfuennmmr.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtyfkieenv.html

[Q71] 查看建表语句
来源：http://hz.yangfankeji.com/gtcmaauscd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jiagoushi.top/gtjbmrttik.html

[Q72] 查看索引
来源：http://hz.nwbrower.top/gtmwetslic.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtfiusyqqm.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gtrqwacnqh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daria6918.cn/gtmuejvutc.html

[Q74] 强制使用索引
来源：http://hz.vqdsnc.cn/gtqlruiqiq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.52xcode.cn/gtorabezau.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtacfrfnwm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gogol.net.cn/gtmneqlwae.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtcafzgcsr.html

[Q76] 按天统计
来源：http://hz.pengpengdd.cyou/gthsxcmmkb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gteavznexs.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtvlnvdzuw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shzxlz.cn/gtenawerqo.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtxrzsmucp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gthohxkjxh.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtglrnpzml.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gtjwkupobn.html

[Q80] 字符串截取
来源：http://hz.jianghu66.top/gtilxhqgta.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ppjwa.cn/gtsdwagqhz.html

[Q81] 字符串替换
来源：http://hz.yj20258888.top/gtmoqwgdjl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jyoumei.cn/gthnomkjns.html

[Q82] 字符长度与字节长度
来源：http://hz.havefunace.top/gtnvhxiuyt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtmbjhswbt.html

[Q83] 大小写转换
来源：http://hz.yj20258.top/gtzkvdrtkx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtxybizgga.html

[Q84] 去除首尾空格
来源：http://hz.havefunace.top/gtbieejvwu.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gtycyqrzrv.html

[Q85] 数值取整
来源：http://hz.wangdashe.top/gtxnqmcmdm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daria6918.cn/gtyuauaxze.html

[Q86] 读取 JSON 字段
来源：http://hz.tanke756.top/gtvtaeuvyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtemvzvaca.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gtvtpheyhg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtpgrddysh.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhiwuduotai.top/gtvgeiakep.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtbberdnha.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtnbwfcsai.html

[Q89] 判断表是否存在
来源：http://hz.xuanzx.com/gtcumdapkg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.bjfxy.top/gthihsnofi.html

[Q90] 生成序号列
来源：http://hz.jinqigufen.top/gtwypuzdfg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtfuexoknq.html

================================================================================
来源：http://hz.nanxinkj.top/gtenceshbv.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtzuhaxpwj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtdflyfbtd.html

[R01] shebang 与严格模式
来源：http://hz.mhx1999.top/gtrachaqjp.html

#!/usr/bin/env bash
来源：http://hz.chenjidiqi.icu/gtgmpukqcc.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtndexqnfm.html

[R02] 变量赋值与使用
来源：http://hz.jyoumei.cn/gtordyryfa.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtekydenck.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gtxtwyjouw.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtrglgrpvp.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtgwnoyhrr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtuoavpiyk.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtaznxbzip.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gtsbacusdx.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtoanfzzsn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtbyngsftk.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtxzngmklf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtiodrmppw.html

[R08] 数值比较
来源：http://hz.vqdsnc.cn/gtafyksfmf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gaohongyu789.top/gtuwksvnmx.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtpdnpydkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtdjktartc.html

[R10] 正则匹配
来源：http://hz.jinyuanbaomall.cn/gtshiquhgc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yangfankeji.com/gtfmuhousv.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtbfqyizxf.html

case "$1" in
来源：http://hz.zhijiandao.cn/gthwbqfupi.html

start) echo "启动" ;;
来源：http://hz.hongshengwenyu.top/gtwrdupgnr.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtjqzpfptd.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtezzevpkx.html

esac
来源：http://hz.jinghuilouyu.cn/gtopjroeep.html

[R12] for 遍历文件
来源：http://hz.cucudq.cn/gtzapgbesm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gtcdeusbhs.html

[R13] for 计数循环
来源：http://hz.jinqigfzy.top/gtgtskalsb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtjoiokcbf.html

[R14] C 风格 for
来源：http://hz.zhixingplan.top/gtkpibowmg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtmlktaetg.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtcgwluymd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guowangkeji.top/gtowjyixxh.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtnrqxycmp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtcbfwrndj.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gtrxxmzwbd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gtwauhviel.html

[R18] 遍历数组
来源：http://hz.guowangkeji.top/gtycxwsdlx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtzuwpiyma.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtcwuafoaq.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtxdvawyja.html

[R20] 关联数组（字典）
来源：http://hz.birdmap.top/gtviqidqmo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gthzgiaeux.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtwnieohsc.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtvdgurkae.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtjnaowbzz.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtfraqrlyd.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtuwmmwcqh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtufmdemkh.html

[R24] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtofomqsvr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtojrrzgnc.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtokuagnlj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sxryk.cn/gtcgdeeixk.html

[R26] 命令替换
来源：http://hz.xziqi.cn/gtllpvovox.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gtcrvoyquq.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtpcadkpjh.html

echo $((1 + 2 * 3))
来源：http://hz.0kj1m.cn/gtxrpjolso.html

[R28] 浮点运算
来源：http://hz.guannengcc.top/gtaxdlyilh.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gttizeqtva.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtwctgrsgd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.kuanghao11.cn/gtgeiflybi.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtyzthhrhs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hysaishi.cn/gtvjergbhi.html

[R31] 局部变量
来源：http://hz.havefunace.top/gtainxbonz.html

f() { local x=1; echo "$x"; }
来源：http://hz.hfpthk.cn/gtwnxnfnxx.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gttlknumir.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtmkdngsgx.html

[R33] 捕获错误并提示行号
来源：http://hz.yangfankeji.com/gtnzbxdach.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtyyoabbfc.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtgauzgqqo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtnnxrggoo.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gtgyumkcex.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtpjfavxhe.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtoqufrmln.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gtfznvnzki.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtejadjqfc.html

files=$(ls -1)
来源：http://hz.hysaishi.cn/gtrapugbrq.html

[R38] 管道串联
来源：http://hz.hnqzz.top/gtuguplcnt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxuanxn.top/gtooasgmwj.html

[R39] 重定向标准输出与错误
来源：http://hz.9152youxi.cn/gtefqzlmgp.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gtekyqvqts.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtjzwgeoql.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtjdhcupas.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtlogxntzx.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtyckwprbf.html

[R42] 输入重定向
来源：http://hz.ydjk.org.cn/gtcqrmuncw.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gtdlquehri.html

[R43] 按名字查找文件
来源：http://hz.hysaishi.cn/gtofqggkwk.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtyodpynbe.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gtrxllfydo.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtszmobhwy.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtqizyfxvh.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtphadrvtl.html

[R46] 递归替换文件内容
来源：http://hz.yangfankeji.com/gtzkrqmias.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.snrcjt.cn/gtbesnjdbx.html

[R47] sed 单行替换
来源：http://hz.ppjwa.cn/gtdqqcfbjl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtxuphbegj.html

[R48] awk 取指定列
来源：http://hz.smart0.xyz/gtpvpqviud.html

awk '{print $1, $3}' a.txt
来源：http://hz.shuidangran.top/gtgajrddgz.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtzotjahjx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtcxpzspti.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtukxhiwad.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aizwys.cn/gtirzcmlez.html

[R51] 排序去重取前几
来源：http://hz.nanxinkj.top/gtfoqjftkp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnqzz.top/gtdcviczed.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtjcihuhyj.html

wc -l a.txt
来源：http://hz.zdqjudy.top/gtfuuptrwg.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gtgazvttvf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.snrcjt.cn/gtynmuwvrs.html

[R54] 比较两个文件
来源：http://hz.jianghu66.top/gtqdoilpsc.html

diff a.txt b.txt
来源：http://hz.jianghu66.top/gtjzvulvgd.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtbzmdwpbq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gteokvrvjv.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtrhlrejkv.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gtvgjppgxu.html

[R57] 远程执行命令
来源：http://hz.hywenlv.cn/gtnpiwtjqr.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtrghjvlro.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtolqbtpnx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gtwemjqexh.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtwffyhgry.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtnqjstdye.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtqicpwkmu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guowangkeji.top/gtlpakflpw.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtkeiaytxz.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gtkexgvmkq.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtafldbxlh.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtuczspwvq.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtwctcqwcj.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtpfvrewdy.html

[R64] 结束进程
来源：http://hz.shuidangran.top/gtdzploukz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtmsbetqbs.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtmfzcaohd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtjqjmkond.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtlggzzxfg.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtoaoajbmr.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtmpnodcsc.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtosrakzsf.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtyjuwnzem.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigufen.top/gtpqeqysgv.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gttgjzphjh.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtgvxythut.html

[R70] 时间戳与互转
来源：http://hz.fzhhl.top/gtlqfhpzss.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtrtymhbcl.html

[R71] 日期格式化
来源：http://hz.fzhhl.top/gtjdqvjrsk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtuepfkmhu.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtvjccoxeq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtooizwzdr.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtpmhasyjj.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtnkhatwjl.html

[R74] 批量重命名
来源：http://hz.snrcjt.cn/gtfpzilpwf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yvedp.cn/gtrdcxlgoe.html

[R75] 导出环境变量
来源：http://hz.daria6918.cn/gthahnnihd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ehwqpu.com/gtznmmbkuu.html

[R76] 使用临时文件
来源：http://hz.nanxuanxn.top/gtzfjraxhz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtuhbjikbc.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtlfllplio.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtwccjoora.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtenqusbrp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtpxecyozv.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gttbpewdbo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.bjfxy.top/gttqepxaog.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtsastffbf.html

time ./run.sh
来源：http://hz.smart0.xyz/gtnikgbwoy.html

================================================================================
来源：http://hz.tianlin.xyz/gtuchcxips.html

S. C / C++ 专题
来源：http://hz.cucudq.cn/gttbouufwu.html

================================================================================
来源：http://hz.tian-w.cn/gtbqzwvjaf.html

[S01] C：Hello World
来源：http://hz.yj20258.top/gtduqouxbr.html

#include <stdio.h>
来源：http://hz.birdmap.top/gtsflczmnl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhaomingkeji.xyz/gtufhmbzba.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtaldgckpt.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtyvmsaeir.html

[S03] C：读入整数
来源：http://hz.shzxlz.cn/gtghojewqr.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtjbfqyfom.html

[S04] C：字符串复制
来源：http://hz.daxiang520.top/gtpxnvwjsl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtfebsyaag.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtijatijey.html

strlen(s)
来源：http://hz.ybcxt.top/gtzrnwhuqt.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gtratpdkcw.html

strcmp(a, b) == 0
来源：http://hz.0kj1m.cn/gtopohytsd.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtcaofnbfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guannengcc.top/gtzpspvtdm.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtpjgoywab.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tanke756.top/gtgdtdszjf.html

[S09] C：结构体定义与初始化
来源：http://hz.hywenlv.cn/gtluoxjfvp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtxnbudjxu.html

[S10] C：指针与解引用
来源：http://hz.zhengqikj.top/gtqwdwtrfs.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtnpjuoeai.html

[S11] C：逐行读文件
来源：http://hz.yj20258.top/gtpprwvbvr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ybcxt.top/gtlvlofcdo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtidlmcffe.html

fclose(f);
来源：http://hz.dashuyun.cn/gtmetwttql.html

[S12] C：写文件
来源：http://hz.yongpay.top/gtwbvdsfzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gtelcrxnft.html

[S13] C：宏定义
来源：http://hz.0kj1m.cn/gtcwzuuhet.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtzunrosfo.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtnawdluqs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtfeauotct.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtrxwzphwn.html

(double) a / b
来源：http://hz.jyoumei.cn/gtfiocbxfj.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gthnnqudhz.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtmcgpnojp.html

[S17] C：安全拼接字符串
来源：http://hz.nanxinkj.top/gtcxkhtadj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigfzy.top/gtnbvdfifh.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtzdgliwfm.html

int main(int argc, char **argv)
来源：http://hz.yj20258888.top/gtkjwexvvc.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gttehryvhq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtxqouqdxl.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gteyubsnje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtnlsichzn.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtaxedxtsa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gtcsxnztrj.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtvfhopgqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tian-w.cn/gtgeriufus.html

[S23] C：随机数
来源：http://hz.shuidangran.top/gtczlwvgxh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtyikwuuqw.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtzwfcezmp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtnvlezkbt.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtxcesjsbv.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtrobijlgv.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtqlgpvyqt.html


<!-- 参考信息 -->
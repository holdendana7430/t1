代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.sufxvd.cn/gtdlqrhuxw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.bjfxy.top/gtzrbcsrvl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yonumen.top/gtlzjabqrm.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtrccucdqe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtksbahwwj.html

[Q50] 批量更新
来源：http://hz.ivvv.top/gtewnsvktn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtdnxvkuee.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtwhsxxoyo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gttsgfkxbu.html

[Q52] 删除指定行
来源：http://hz.cqqwz.cn/gtqfbxdtjz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtpasyadaq.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtuqliqiam.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.meibo888.top/gtcvxwlzgg.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtvznckzke.html

TRUNCATE TABLE logs;
来源：http://hz.zhiwuduotai.top/gtiyghrpnl.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtdmmwarse.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yangfankeji.com/gtjtkzckrs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gtqtgssuxk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtcqcbqrdz.html

[Q57] 行号
来源：http://hz.daria6918.cn/gtpzfygdad.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtbjxiephy.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gtmnoanxuq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gtmvndxcqm.html

[Q59] 分组内累计
来源：http://hz.daria6918.cn/gtaomkrisv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258888.top/gtqjpkaouf.html

[Q60] 取上一行 / 下一行
来源：http://hz.sufxvd.cn/gtnzpchvql.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtcfzdlouw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yongpay.top/gtntnnfyfz.html

[Q61] 移动平均
来源：http://hz.xuetiantiany.cn/gtcqkelfxf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtdbvzzqoh.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtyzikgxne.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtkkgbpigz.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtafmfqqtg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtgumwsmnv.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtfysxronk.html

COMMIT;
来源：http://hz.jinqigfzy.top/gtrwezeisc.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtzifnxhnf.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtgnstbcgn.html

[Q66] 行锁查询
来源：http://hz.shzxlz.cn/gtnnggnqpk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtpcaslink.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtsvhixwli.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gtakxkonhb.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtbilmzrnp.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gtoycozdpf.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtphdpnote.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtshnagngo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dashuyun.cn/gtuybrlqgf.html

[Q70] 更新统计信息
来源：http://hz.tian-w.cn/gtltaijjlr.html

ANALYZE TABLE users;
来源：http://hz.daria6918.cn/gtmvyedolb.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtgptisboj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hfpthk.cn/gtpvrywagd.html

[Q72] 查看索引
来源：http://hz.hongshengwenyu.top/gtcfeuumkj.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtqigjxzdk.html

[Q73] 查看表状态
来源：http://hz.tanke756.top/gttfdkiezx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yueranfly.top/gtfgjfohdd.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtavcletzw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxinkj.top/gtkedevxvs.html

[Q75] 日期格式化
来源：http://hz.fengsongda.top/gtvmbvictx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhoulong.xyz/gtnwpudvnw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ehwqpu.com/gtyivbzahp.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtmisciikv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtsyymmmea.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gthrdthxpl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xylfe.cn/gtaaumhhda.html

[Q78] 当前时间
来源：http://hz.haohaochexian.top/gtezuupsaw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtzjjwgnuc.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtahlpulba.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.andypj.xyz/gtjxfvpuuw.html

[Q80] 字符串截取
来源：http://hz.hnqzz.top/gtametadpg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtkumxucic.html

[Q81] 字符串替换
来源：http://hz.redwolf501.top/gtrkpopgcr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtraizgkhh.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtarrlqdqc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jianghu66.top/gtzaxthmmv.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtvdywawdr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtzhotnupu.html

[Q84] 去除首尾空格
来源：http://hz.vqdsnc.cn/gtwpnrsiwn.html

SELECT TRIM(name) FROM users;
来源：http://hz.aizwys.cn/gtgrsbaage.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtjekffptz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnxiangtu.top/gtrjmutxrj.html

[Q86] 读取 JSON 字段
来源：http://hz.havefunace.top/gtijnpomqy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yangfankeji.com/gteysezhac.html

[Q87] JSON 字段做条件
来源：http://hz.gotoacloud.top/gtosgdnlgu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cdnleiting.top/gtemhoeacj.html

[Q88] 行转列（条件聚合）
来源：http://hz.guannengcc.top/gthxmxqaid.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtxdbmwwof.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenjidiqi.icu/gtmtuvguzc.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtqlctogwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gtpxjgbqne.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtefygercg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gtrqedrrxy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdbielirp.html

R. Bash 专题
来源：http://hz.iojbl.cn/gttneiexel.html

================================================================================
来源：http://hz.yj202588.top/gtpctdymfl.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtqsyhohwr.html

#!/usr/bin/env bash
来源：http://hz.hywenlv.cn/gtpdvbzmos.html

set -euo pipefail
来源：http://hz.guowangkeji.top/gtdxlyafcg.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtsiroykxa.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gtflhqgmes.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtntdmooxb.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtgflmcczw.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtzuutwqcf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtikzryepm.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtjnmdtxmi.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gtzrhidwch.html

[R06] 判断命令是否存在
来源：http://hz.ivvv.top/gtjjgjrvzz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtdyenbpoc.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gthxclmwev.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zdqjudy.top/gtdjccbamu.html

[R08] 数值比较
来源：http://hz.cashguo.top/gttqoucppm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtczbapadu.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtiefyvzhx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258.top/gthbdocibq.html

[R10] 正则匹配
来源：http://hz.shzxlz.cn/gtesxiyrdo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtrfoomuiq.html

[R11] case 多分支
来源：http://hz.ivvv.top/gtzzrzdnqc.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtmlajeulp.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtguauqfjz.html

stop)  echo "停止" ;;
来源：http://hz.smart0.xyz/gtkhhadakj.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gtqiftxlso.html

esac
来源：http://hz.gaohongyu789.top/gtlusctwvd.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtkrqifamn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxinkj.top/gtwnjpiotr.html

[R13] for 计数循环
来源：http://hz.gzhubu.top/gtnkahnhae.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hammf.cn/gtauixlxks.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtpzxbjjit.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtnukafbbi.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtuvoliadm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gtctfzhwcl.html

[R16] until 等待条件
来源：http://hz.zdqjudy.top/gtuoipojfu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxuanxn.top/gtkicchhjc.html

[R17] 数组定义与取值
来源：http://hz.daria6918.cn/gtboomoxew.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtzexzabri.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtgdvjzlff.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gtgeyqpmtr.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtnvscqqyv.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gteojstbts.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gtpepqnrdi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtbnxtwrpk.html

[R21] 字符串长度
来源：http://hz.aibaodan.cn/gtgircfekj.html

echo "${#s}"
来源：http://hz.hnqzz.top/gthupcqsxm.html

[R22] 截取子串
来源：http://hz.chenlongwang.top/gtjyltzgft.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtyajspuia.html

[R23] 字符串替换
来源：http://hz.hammf.cn/gtxioszipr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtjpuqfaxk.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtznxfkfoo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tianlin.xyz/gtpiluruss.html

[R25] 去后缀 / 去前缀
来源：http://hz.snrcjt.cn/gtagymwyem.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gaohongyu789.top/gtcigjhwsi.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtayehytyq.html

now=$(date +%F); echo "$now"
来源：http://hz.cashguo.top/gtirrvboru.html

[R27] 算术展开
来源：http://hz.xuanzx.com/gtkpwcejeq.html

echo $((1 + 2 * 3))
来源：http://hz.xingfuxueyuan.xyz/gtvhvwsitg.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtamkgkuim.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gtzvieocpv.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtnayltpcx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtconuffaz.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gtibjcbghd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.birdmap.top/gtijkyoxaz.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtibdmzhpr.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtykrhrpmg.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtxephddxq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xinyue.icu/gttbaycfcn.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtlrwsmrve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtvzheecxi.html

[R34] 退出时清理
来源：http://hz.kuanghao11.cn/gtkvvzifas.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtqjuxajkn.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gterepscal.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gzhubu.top/gttwlsdqff.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtpomrmlgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sufxvd.cn/gtggpwzrck.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtgxfladss.html

files=$(ls -1)
来源：http://hz.zhoulong.xyz/gthcklcxmj.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtbblqcvnu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cucudq.cn/gtwbnuzwxp.html

[R39] 重定向标准输出与错误
来源：http://hz.chenlongwang.top/gtpyqkvovu.html

cmd > out.log 2>&1
来源：http://hz.gaohongyu789.top/gtnamfkoti.html

[R40] 追加写日志
来源：http://hz.pycfn.com/gtkxtuzknz.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gtcqsmacrs.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtvvzciqwz.html

cmd >/dev/null 2>&1
来源：http://hz.yangfankeji.com/gtppdaudkv.html

[R42] 输入重定向
来源：http://hz.zhijiandao.cn/gtbbicalfr.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtmsmawdwc.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gteoedjbpr.html

find . -name "*.log" -type f
来源：http://hz.xuanzx.com/gtboxnewsx.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gterlqcrnj.html

find . -mtime -7 -type f
来源：http://hz.meibo888.top/gtlbzjnweo.html

[R45] 批量删除
来源：http://hz.zhijiandao.cn/gtnvortcnh.html

find . -name "*.tmp" -delete
来源：http://hz.nwbrower.top/gtpizsyizv.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gthmopcwhj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gzhubu.top/gtkqlxdics.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtjnyijqzx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtifxssyae.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtfmeuhkbs.html

awk '{print $1, $3}' a.txt
来源：http://hz.tian-w.cn/gtbrsqxdpw.html

[R49] awk 带条件
来源：http://hz.jinghuilouyu.cn/gtclssrksr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtrkqbdsab.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtdmdumuko.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtwrnhvzrn.html

[R51] 排序去重取前几
来源：http://hz.chenjidiqi.icu/gttygrehfw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtklewwvzc.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtdxqcdcne.html

wc -l a.txt
来源：http://hz.daxiang520.top/gtqsmtupse.html

[R53] 查看文件头与实时尾
来源：http://hz.cashguo.top/gtkthmdqbz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtosuwjpru.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gthvirnprf.html

diff a.txt b.txt
来源：http://hz.0kj1m.cn/gtmamrnwuo.html

[R55] 压缩与解压
来源：http://hz.hnxiangtu.top/gtmficgeko.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtnpfdxyul.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gtayvxecnn.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtfjomqcnc.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtmmsoivjn.html

ssh user@host 'uptime'
来源：http://hz.birdmap.top/gtsyllutoz.html

[R58] 下载文件
来源：http://hz.andypj.xyz/gtlcfrepig.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtvncgrbeb.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtxonzwfqm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtdkhkjxjs.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenzaomai.com/gtaytvrffx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gthpvjspia.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtaroitxhg.html

df -h;  du -sh *
来源：http://hz.ehwqpu.com/gthdynrxpv.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtdozmvpow.html

du -ah . | sort -rh | head -10
来源：http://hz.ppjwa.cn/gtrtntlyth.html

[R63] 内存与进程
来源：http://hz.kuanghao11.cn/gtlntbdijb.html

free -h;  ps aux | grep nginx
来源：http://hz.sxryk.cn/gtlrvndhoz.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtmqrhinjo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gteaokmzeh.html

[R65] 查看端口占用
来源：http://hz.yanxiufei.cn/gtslewezwo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhiwuduotai.top/gtmamzqroe.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtnldetlvh.html

crontab -e;  crontab -l
来源：http://hz.xingfuxueyuan.xyz/gtmkxpsobb.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtvqwtxcbk.html

openssl rand -hex 16
来源：http://hz.havefunace.top/gtjyxvyoaq.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtodwlupcj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtimcpvqdd.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gtazkyhltt.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtwfplapax.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gthqtbztqf.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtxlkmtobs.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gthdltnktl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gtkmhrreiv.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtefpcshxi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtgxevditi.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtnraxyhhm.html

split -l 1000 big.log part_
来源：http://hz.hfpthk.cn/gtmxrgfrvc.html

[R74] 批量重命名
来源：http://hz.snrcjt.cn/gtpjzunpkj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtpgwrzgww.html

[R75] 导出环境变量
来源：http://hz.xziqi.cn/gtxhejlnuo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtdiwhforo.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtygqjhdsl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtjropfsxu.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangtech.top/gtfciauokt.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtxgagjdmi.html

[R78] 交互式菜单
来源：http://hz.hywenlv.cn/gtotktpcut.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fzhhl.top/gttsbxsfwp.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtrcrwoybx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtngmgxcmf.html

[R80] 查看脚本执行耗时
来源：http://hz.vqdsnc.cn/gthtdyhmhe.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gtfczueebj.html

================================================================================
来源：http://hz.hfpthk.cn/gtzguozvzm.html

S. C / C++ 专题
来源：http://hz.fengsongda.top/gtcletgzvp.html

================================================================================
来源：http://hz.guannengcc.top/gterpfuyel.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gtzqjdmrqs.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gtpzbklygj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258.top/gtentknnwx.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtlcnozcud.html

int a = 10; printf("%d\n", a);
来源：http://hz.xziqi.cn/gthriavbvj.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtvxcvpbmt.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtdssskdyy.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtqqtecfuo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dianchejie.cn/gtpxzjqzxg.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtbrokjuhz.html

strlen(s)
来源：http://hz.zhengqikj.top/gttadrsxnp.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtobamfuft.html

strcmp(a, b) == 0
来源：http://hz.52xcode.cn/gtfovpuwib.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtkreckkct.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhiwuduotai.top/gtefejunex.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtsihbeaip.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hammf.cn/gttgvblsqv.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtwoapbiff.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhiwuduotai.top/gtvxyxttlm.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtdytaspto.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtqkhvkxvf.html

[S11] C：逐行读文件
来源：http://hz.yuanzhike.top/gtqhbcibax.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtzgyudxvl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gtnkzoxtby.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtjxwybfoh.html

[S12] C：写文件
来源：http://hz.kuanghao11.cn/gtkuezwnfz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fengsongda.top/gtvqxlhjbu.html

[S13] C：宏定义
来源：http://hz.yj202588.top/gtziatlwav.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtzuzsuwwb.html

[S14] C：枚举
来源：http://hz.jinqigfzy.top/gtnuquuren.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gtuuuqszvo.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtzkmewalm.html

(double) a / b
来源：http://hz.nanxuanxn.top/gtqjpdprqo.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtmbrldvfm.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtxfumkext.html

[S17] C：安全拼接字符串
来源：http://hz.yonumen.top/gtordxgkmx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gttzdfxkhs.html

[S18] C：命令行参数
来源：http://hz.jinqigufen.top/gtyuzqeusg.html


<!-- 参考信息 -->
代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinyuanbaomall.cn/gtigxxsxib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtqworwele.html

[Q47] 与平均值比较
来源：http://hz.shuidangran.top/gtsajlebak.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gogol.net.cn/gtrjvqkiyi.html

[Q48] CTE 公用表表达式
来源：http://hz.fengsongda.top/gtmpobfpek.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xylfe.cn/gtpwrrwdnw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtmnnibyoo.html

[Q49] 更新单行
来源：http://hz.feifeiyinyue.top/gtmistfwfy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtafhaldbu.html

[Q50] 批量更新
来源：http://hz.iojbl.cn/gtjgvixjne.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gttryjhxks.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtfgcwefsj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtpyhpyxnq.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gthinwzzbi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gtfaowpmlf.html

[Q53] 按条件删除
来源：http://hz.c1oappe.top/gtyexblytk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigfzy.top/gtagdrwztr.html

[Q54] 清空表
来源：http://hz.quarkkingdee.top/gtydjqkewm.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gtebncmnhb.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtoevbgqsn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnqzz.top/gtokwlvdvl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenjidiqi.icu/gticxajqjo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zdqjudy.top/gtuzpgxtri.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtnbmlxwwv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtbuxibthg.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtuipjuaua.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangshuangyany.cn/gtydijcdog.html

[Q59] 分组内累计
来源：http://hz.nwbrower.top/gtbeikrmvp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhengqikj.top/gtbeoplgwk.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtkjhrukpc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtflwmsqzv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtrbpbfstr.html

[Q61] 移动平均
来源：http://hz.jinyuanbaomall.cn/gtrqxijiuh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hongshengwenyu.top/gtwrnyefaj.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtcwsxmnrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtmhnthjmd.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtljnsvjvr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtqhczdykc.html

[Q64] 提交事务
来源：http://hz.yueranfly.top/gtrohsdkdp.html

COMMIT;
来源：http://hz.chenlongwang.top/gtffzgmbdr.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtugceunik.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtwkhslyhs.html

[Q66] 行锁查询
来源：http://hz.guowangkeji.top/gtfowcedat.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtwnrbwily.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtsecnaqkm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtwetwurxy.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtghhvqumh.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtfsxlzypa.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtkafllddw.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtqodujhec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.haohaochexian.top/gtiwamikva.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtqzgaxuau.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtrtwcsspo.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtylqqfxzl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gttkikyveq.html

[Q72] 查看索引
来源：http://hz.nanxuanxn.top/gtvglyftpc.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtzafcjwtq.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtfbunmibx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtxedtviuw.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtzlrtriyl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtjatmprnu.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtylggnevs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aibaodan.cn/gtxhfegrql.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tanke756.top/gtfwxranwj.html

[Q76] 按天统计
来源：http://hz.daxiang520.top/gtbjfwweiw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gzhubu.top/gteewvfrtq.html

[Q77] 时间加减
来源：http://hz.jlsjyb.cn/gtrpbnpgrx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gotoacloud.top/gtkjayakla.html

[Q78] 当前时间
来源：http://hz.jlsjyb.cn/gtnrwszbmt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jianghu66.top/gtjepwvhqm.html

[Q79] 字符串拼接
来源：http://hz.birdmap.top/gtysgodxen.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtujznrtax.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtmcplspsp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtlycinvox.html

[Q81] 字符串替换
来源：http://hz.xuanzx.com/gtmudgglet.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtzfdxcmib.html

[Q82] 字符长度与字节长度
来源：http://hz.birdmap.top/gtiypyiwsu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtdjgubsdg.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtztrocejb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shzxlz.cn/gtzooriomc.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtougknhhq.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxuanxn.top/gtcezwtefq.html

[Q85] 数值取整
来源：http://hz.shangyingyoupin.top/gtsasnthwe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtyzknfulr.html

[Q86] 读取 JSON 字段
来源：http://hz.pycfn.com/gtikcuffxj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtrxrzpfpu.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gttaefqxqy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.vqdsnc.cn/gtreizmgxf.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinghuilouyu.cn/gtbdpsqrnf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gtvbzlduzg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gtdzyrdtqn.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtwbsgzpgn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtrvlokylq.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtsxmsuwky.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.andypj.xyz/gtkbcncbwd.html

================================================================================
来源：http://hz.haohaochexian.top/gtxcnxiddb.html

R. Bash 专题
来源：http://hz.shuidangran.top/gtupjrjpru.html

================================================================================
来源：http://hz.chenlongwang.top/gterhxbtlh.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtfjovlxgh.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtsbtwiblf.html

set -euo pipefail
来源：http://hz.shanyushiyangkeji.top/gtsrtahknd.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtobqskqcb.html

name="Tom"; echo "$name"
来源：http://hz.cqqwz.cn/gtnuvyhfez.html

[R03] 只读变量
来源：http://hz.yanxiufei.cn/gtvessesys.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtnuusjuge.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtgidzistj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258888.top/gtgkbmeayq.html

[R05] 参数默认值
来源：http://hz.tianlin.xyz/gtsortazou.html

name="${1:-default}"
来源：http://hz.jinghuilouyu.cn/gtpadbdqyy.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtsdrrnhjc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtexlujgul.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtxfractei.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhengqikj.top/gtznmfcftj.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtlizctrog.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.snrcjt.cn/gtbxwzxnis.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtjyumuqqq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gthwnuknfp.html

[R10] 正则匹配
来源：http://hz.c1oappe.top/gtbunekomo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.9152youxi.cn/gtbgxynfzi.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtxkrgiarh.html

case "$1" in
来源：http://hz.52xcode.cn/gtwqzvpvti.html

start) echo "启动" ;;
来源：http://hz.jinqigufen.top/gtbeoenxzi.html

stop)  echo "停止" ;;
来源：http://hz.tanke756.top/gtbtjgwmfn.html

*)     echo "未知命令" ;;
来源：http://hz.jinyuanbaomall.cn/gtvkfmxbmz.html

esac
来源：http://hz.aizwys.cn/gtbkgincnc.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtiwkwxeyq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.bjfxy.top/gtxqahobnd.html

[R13] for 计数循环
来源：http://hz.aibaodan.cn/gtgtgntvuv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jianghu66.top/gtcblciysx.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtbhdgphff.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ehwqpu.com/gtylrhhgem.html

[R15] while 逐行读文件
来源：http://hz.yongpay.top/gtpzkiberm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ivvv.top/gtycbxaewz.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gtkqsvylaq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hywenlv.cn/gttwmjqoun.html

[R17] 数组定义与取值
来源：http://hz.guannengcc.top/gtfpqwgega.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuanzx.com/gtobqusvsa.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtbsadaznc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtjzqwtgud.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtghfvaapd.html

echo "${#arr[@]}"
来源：http://hz.zdqjudy.top/gtbkfijkmi.html

[R20] 关联数组（字典）
来源：http://hz.nwbrower.top/gtjssccftn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gterttnuas.html

[R21] 字符串长度
来源：http://hz.daxiang520.top/gtplqdnfeq.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtvzougpxl.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gthcbvlgxo.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gtqcfwcxza.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gtrdcwmpry.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gtmhwchqli.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtalunadxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.redwolf501.top/gtfhibrvrr.html

[R25] 去后缀 / 去前缀
来源：http://hz.ybcxt.top/gttajuqgsn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtokoznakj.html

[R26] 命令替换
来源：http://hz.pengpengdd.cyou/gtfgdfyeqd.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gtgtbwahud.html

[R27] 算术展开
来源：http://hz.yanxiufei.cn/gtbspufjac.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtrfimstgf.html

[R28] 浮点运算
来源：http://hz.tian-w.cn/gtkrcsketp.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtnbfhzaiz.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtpcthnzsa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtnlmezddo.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gtmhsqbcoa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gtyfllsbvg.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtrvpbhavk.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gtkwagqwag.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtvqsvahdk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtnrdeomat.html

[R33] 捕获错误并提示行号
来源：http://hz.iojbl.cn/gtfyvdwyct.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtxbsvglju.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gtrmwksqua.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtrupvqosf.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtbygauukh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtvqcgtwic.html

[R36] 并发执行多个任务
来源：http://hz.haohaochexian.top/gtggxdcgge.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258888.top/gtdngitsls.html

[R37] 把输出赋给变量
来源：http://hz.yj202588.top/gtouqiyaew.html

files=$(ls -1)
来源：http://hz.haohaochexian.top/gtrjwuadtv.html

[R38] 管道串联
来源：http://hz.zhixingplan.top/gtaoquwenz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hfpthk.cn/gtglgtvdnb.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gteihpjcfo.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gtsjqgykgf.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtsszkjysg.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtbpvlikbs.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtmstftqat.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtxclfrpcu.html

[R42] 输入重定向
来源：http://hz.yonumen.top/gtakqhrwwz.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtvcxpotml.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gtvyacuihs.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtogpkwvsp.html

[R44] 按修改时间查找
来源：http://hz.nanxuanxn.top/gtoqtiujzs.html

find . -mtime -7 -type f
来源：http://hz.yangfankeji.com/gtjtnxxtzq.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtigakvjnv.html

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtlandhcak.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtofqxovua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aibaodan.cn/gtoowijzks.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtatxnwfry.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtipofazau.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtvveiouag.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtlqjsgrjv.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtdgnlwgdq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuanzhike.top/gtpyfbeaxf.html

[R50] awk 求和
来源：http://hz.yj202588.top/gtzilcznln.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dashuyun.cn/gtwqicdsnx.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtynwbnozc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhijiandao.cn/gtvvuyhowf.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtpiwkirgh.html

wc -l a.txt
来源：http://hz.fengsongda.top/gtmamoshir.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtdlxnhthi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hywenlv.cn/gtbkgstbfv.html

[R54] 比较两个文件
来源：http://hz.kuanghao11.cn/gtsyowaofr.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtpqffmugm.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtvtlbrkjy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gttdjgjtpq.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtcfcuzxqd.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtwcrqgxoq.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtlmidijyc.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtjjirjfqe.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gthhqfyciq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtrdldwjfr.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gteryfqzhh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtalyfdxzm.html

[R60] 只看 HTTP 状态码
来源：http://hz.yvedp.cn/gtxiczlxej.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aibaodan.cn/gtwxvndhar.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtgvpqpeuc.html

df -h;  du -sh *
来源：http://hz.zhengqikj.top/gtrfgrwilj.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gtovbxkqnp.html

du -ah . | sort -rh | head -10
来源：http://hz.aibaodan.cn/gtwsibdsml.html

[R63] 内存与进程
来源：http://hz.xziqi.cn/gtwemzybtm.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtkvjbnowb.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtglecpecx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gttayxfpwk.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtqhjhfdix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtvsyftdbb.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtpnsplhsm.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtzucpblxt.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtjwfonbqr.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtkpkzgfph.html

[R68] 计算文件校验值
来源：http://hz.jinqigufen.top/gtqqslskto.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jiagoushi.top/gtxyybpbpg.html

[R69] 生成随机密码
来源：http://hz.zhoulong.xyz/gtldderezy.html

head -c 16 /dev/urandom | base64
来源：http://hz.ehwqpu.com/gtuykdfvhg.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtaqkyuyrx.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtfqktgnch.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtzzvkbjfq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtdeclesxp.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtxnbbydbl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtfqwwzgzs.html

[R73] 分割大日志
来源：http://hz.jinqigfzy.top/gtvelhmxvb.html

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gttodcmnij.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtdbsotouo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigufen.top/gtwpdqrjbn.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtqsmqiqnw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gthpgeoule.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gtcyjlefaj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtjlqujoux.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtybgqqfzl.html

read -rp "请输入: " ans
来源：http://hz.yuxming.cn/gtayqyxqes.html

[R78] 交互式菜单
来源：http://hz.haohaochexian.top/gteaqrefox.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtvzptgxhs.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gttkxizktc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtgfhqnwrz.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtimxqljzr.html

time ./run.sh
来源：http://hz.daria6918.cn/gtkvrdvzpn.html

================================================================================
来源：http://hz.cqqwz.cn/gtsrbcyzec.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtxugvgteu.html

================================================================================
来源：http://hz.sufxvd.cn/gtuxqiqwmi.html

[S01] C：Hello World
来源：http://hz.wangdashe.top/gtmkcufaiy.html

#include <stdio.h>
来源：http://hz.xziqi.cn/gtefuhvsgi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtcnazgehz.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtcxnmadqg.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigfzy.top/gttqwdduqv.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtsxempbjj.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtligwwvig.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gthomxruns.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangkeji.top/gtzvskabhf.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtkxzaiwvo.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtmzlzsjtf.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtxlvmaifz.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtppwqnqlv.html

[S07] C：数组遍历求和
来源：http://hz.chenlongwang.top/gtxszrfage.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.bjfxy.top/gtpskruqsv.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtxgympyjt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sweek.top/gtegkxgdlt.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtylddjbiw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jyoumei.cn/gtvpglwyrd.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtlrkmgfdd.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtwpifwphq.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtsrbwucmi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xingfuxueyuan.xyz/gtcyrkjojf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.birdmap.top/gttutadlee.html

fclose(f);
来源：http://hz.yonumen.top/gtwtlkhmtg.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtneeflluz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtxupiwgly.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtlyfgsbnu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtftzydfvk.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtztpdrheq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cdnleiting.top/gtenzlnqmy.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtyrlyilqp.html

(double) a / b
来源：http://hz.yueranfly.top/gtwgskoadm.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtlkvzmrsc.html


<!-- 参考信息 -->
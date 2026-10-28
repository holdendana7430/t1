代发 wailian999

[Q36] 左连接
来源：http://hz.wangshuangyany.cn/gtlrnfelyp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtdfvxzvhd.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gtjnhgstyk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sxryk.cn/gtujsgxaqe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtafebzwua.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yonumen.top/gtzjferara.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtfcjnxwta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tian-w.cn/gtvdceuzot.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yangfankeji.com/gtslcpvqlb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtiqhexmit.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtjrkrfgqz.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtatujpqdb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yvedp.cn/gtrngrkxud.html

JOIN users u ON u.id = o.user_id
来源：http://hz.kuanghao11.cn/gtvwgnmpmb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtnpbrfvga.html

[Q42] 连接条件附加过滤
来源：http://hz.vqdsnc.cn/gtkuumttkt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtczpkoqhk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhoulong.xyz/gtziepazzy.html

[Q43] 标量子查询
来源：http://hz.andypj.xyz/gtqsotkubj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gteceuddue.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gtrrdnkmhv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtzhhxfwor.html

[Q45] EXISTS 判断存在
来源：http://hz.ywan-chungtsiang.top/gthrrtiqeh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtbajjbjot.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.quarkkingdee.top/gtrdmgnqqs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gthhvypfje.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtfizchfov.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.guannengcc.top/gtmvvpscjz.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtwshizsbd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtyfhkrnet.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtuzecsjbk.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtuijntynw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtojqymbdv.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gtvxowbmyz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gtynejnmey.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtryqipezn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtdjguifly.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gttjdaxxpx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtkxbtxych.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gtcosxexcw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fengsongda.top/gtunwnnxjj.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtlvxjqdhw.html

TRUNCATE TABLE logs;
来源：http://hz.cqqwz.cn/gtuapcsoea.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtagpohyqy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtbfflgezw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cdnleiting.top/gtzmouuxsg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xingfuxueyuan.xyz/gthjkfrpwb.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gtsivujuck.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sxryk.cn/gtvgkkginn.html

[Q58] 累计求和
来源：http://hz.zycfv.cn/gtcsndvjwy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtxewnqlps.html

[Q59] 分组内累计
来源：http://hz.zhixingplan.top/gtkjgvzrsn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtxmqshbna.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnxiangtu.top/gthmiyvflo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gthrskdbeu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxinkj.top/gtgszwbbue.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtwctktvqp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtpkktiqee.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtjpizixrc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtkmeecmvt.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtskhgndlb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cashguo.top/gtkmmjdtlb.html

[Q64] 提交事务
来源：http://hz.52xcode.cn/gthifpnors.html

COMMIT;
来源：http://hz.pycfn.com/gtcyhafuox.html

[Q65] 回滚事务
来源：http://hz.hywenlv.cn/gtjjlsjsqo.html

ROLLBACK;
来源：http://hz.zdqjudy.top/gtztplycpt.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtcinlotxb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydzc1.top/gtnqztqfxi.html

[Q67] 设置隔离级别
来源：http://hz.snrcjt.cn/gtpubkuhsu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigufen.top/gtqgorcdtr.html

[Q68] 保存点
来源：http://hz.ybcxt.top/gtipynrqil.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtlcligiax.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtfugtmrgx.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtjulcobxz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zdqjudy.top/gtawtoftwi.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtnremjzjx.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtmsbbuzvp.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gtqygdgyht.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtrglxnvrf.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gtjzfzsnzu.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtyaimfwzv.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtoejuywmw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gthjegwazk.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtbwefprne.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gtobfcffyu.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtrqjltarn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.smart0.xyz/gtwlastdqj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtmzwsqbvl.html

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gtlnmdiirv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenlongwang.top/gtsnzsgfgy.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtfjicnyuj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gtlljxojvi.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtacvvtqhn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yueranfly.top/gtsfkngjeb.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gteldfdozv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tanke756.top/gtdwzywzxl.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gthhdvziha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxinkj.top/gtdvgybflg.html

[Q81] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gthdotcuqb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fzhhl.top/gtphtrormv.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtsshlnexk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtpfpaopyx.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtsqdsyiet.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtuslilrgb.html

[Q84] 去除首尾空格
来源：http://hz.xziqi.cn/gtaswcvpda.html

SELECT TRIM(name) FROM users;
来源：http://hz.fzhhl.top/gtgjqkduyb.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtcgouxlji.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.meibo888.top/gtyeldtavu.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtmbqtdjja.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtqhyymyxz.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gtnehmpdzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gtohceltyt.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtuibelosj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.vqdsnc.cn/gtwzuemluz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtnedwfqwo.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtivekdnjv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtyireatbx.html

[Q90] 生成序号列
来源：http://hz.aibaodan.cn/gtcydpxgum.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sxryk.cn/gtcmdaexfv.html

================================================================================
来源：http://hz.ydzc1.top/gtbuyboelm.html

R. Bash 专题
来源：http://hz.ydjk.org.cn/gtdegftphh.html

================================================================================
来源：http://hz.havefunace.top/gtiefkbcaw.html

[R01] shebang 与严格模式
来源：http://hz.nwbrower.top/gtnkbklbpy.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtwibzjaym.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtyxopvbeh.html

[R02] 变量赋值与使用
来源：http://hz.nanxuanxn.top/gtahpcosnl.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtkyttagzf.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtclcwdwwn.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtcqroncvq.html

[R04] 位置参数
来源：http://hz.kuanghao11.cn/gtsnzdfdgd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtzzxrenwv.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtvbfzrscv.html

name="${1:-default}"
来源：http://hz.sysykeji.top/gtkanosllq.html

[R06] 判断命令是否存在
来源：http://hz.hfpthk.cn/gtdfugklwm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtgsjnlxej.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gttxewvsps.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.316326.xyz/gtldxmaham.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtkcyjatuk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtmfetjlpr.html

[R09] 字符串比较
来源：http://hz.jyoumei.cn/gtzsuhyxfy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtxcqwenqs.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gttzgtwwus.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtltzqbrnq.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtdcmtegfm.html

case "$1" in
来源：http://hz.cucudq.cn/gtkqywsrlx.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gttngqvrqn.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtojfrehjn.html

*)     echo "未知命令" ;;
来源：http://hz.shangyingyoupin.top/gtwmuvbxue.html

esac
来源：http://hz.feifeiyinyue.top/gtsmybqnmb.html

[R12] for 遍历文件
来源：http://hz.quarkkingdee.top/gthaimdmdi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtbheqyhhl.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtlpffpcyk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtzxzwawte.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtractukpb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuxming.cn/gtrcvarpld.html

[R15] while 逐行读文件
来源：http://hz.shzxlz.cn/gtehitisfk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtexlowpts.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtbqarauvg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtsaofxixu.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtbqcuddlj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtnpckggfg.html

[R18] 遍历数组
来源：http://hz.shanyushiyangtech.top/gtxdgoitia.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtjfiixfjg.html

[R19] 数组长度
来源：http://hz.zdqjudy.top/gtnpjjfmol.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtszpsefow.html

[R20] 关联数组（字典）
来源：http://hz.ydjk.org.cn/gtglwseygu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gtgeupkvnt.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtzpycyipz.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtomzeuaoj.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtdvxkpeuc.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtmqcubkdq.html

[R23] 字符串替换
来源：http://hz.ydjk.org.cn/gtbwudrxfh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangtech.top/gtehplhgfq.html

[R24] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtghynfmmr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtunsrgolf.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtngzukxfk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.quarkkingdee.top/gteyploshi.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtfqqbmlfq.html

now=$(date +%F); echo "$now"
来源：http://hz.guannengcc.top/gtqgudblqk.html

[R27] 算术展开
来源：http://hz.shanyushiyangkeji.top/gtdlanxbqf.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtikgigrfv.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtvsepvifh.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtrzogwikq.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gthomnonks.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gtwhcmudnu.html

[R30] 函数返回状态码
来源：http://hz.hywenlv.cn/gtkbhyyiqz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.havefunace.top/gtnjvrmmrb.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gtgvmairlw.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtbpugzzxv.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtwocmckva.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hongshengwenyu.top/gthyfscrrp.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtmajhncad.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gtqegxbbhh.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtbieuiprh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtompjglqj.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gthszutmet.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtxwohzodr.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gtfepcpwss.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtwxvrrnrj.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtfksxzqrg.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtzkjznybg.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtmxccblxp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guannengcc.top/gtrmojnfri.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtnqmzhwdp.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtcfbelzus.html

[R40] 追加写日志
来源：http://hz.hnxiangtu.top/gtgudwiyfl.html

echo "log" >> out.log
来源：http://hz.zycfv.cn/gtywxzglsv.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gtekxqbmnp.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtjeblzvrd.html

[R42] 输入重定向
来源：http://hz.zhengqikj.top/gttjqtfshr.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtecfvngvv.html

[R43] 按名字查找文件
来源：http://hz.ivvv.top/gtzrjyfanz.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtntmaunmz.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gtymtgjspm.html

find . -mtime -7 -type f
来源：http://hz.gotoacloud.top/gtkdbiyrll.html

[R45] 批量删除
来源：http://hz.aibaodan.cn/gtqggssnkr.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtcwhiclqh.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtqxgeokxz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtvzdtennh.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtrtboappd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuanzx.com/gtrxjvbgck.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtnvwzqdsl.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtsorzxvdt.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtudarxapv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangshuangyany.cn/gtzebwmzbh.html

[R50] awk 求和
来源：http://hz.ydjk.org.cn/gtogxdqxpu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtjqhvsxbo.html

[R51] 排序去重取前几
来源：http://hz.yvedp.cn/gtfzienzcr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gtqxiaoura.html

[R52] 统计行数
来源：http://hz.andypj.xyz/gtsjrervlc.html

wc -l a.txt
来源：http://hz.52xcode.cn/gtokezwhrv.html

[R53] 查看文件头与实时尾
来源：http://hz.gotoacloud.top/gtlkhjvtgl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuanzx.com/gtnoternjk.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtglnvwucq.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtuarerlsp.html

[R55] 压缩与解压
来源：http://hz.shzxlz.cn/gtyakxwwzi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gaohongyu789.top/gtlqulkrds.html

[R56] 远程拷贝
来源：http://hz.sysykeji.top/gtphxldhpw.html

scp file user@host:/path/
来源：http://hz.havefunace.top/gtcdqijnto.html

[R57] 远程执行命令
来源：http://hz.pengpengdd.cyou/gtkhdtowfe.html

ssh user@host 'uptime'
来源：http://hz.birdmap.top/gtvjqwwkeq.html

[R58] 下载文件
来源：http://hz.bjfxy.top/gtvlcpszvc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.9152youxi.cn/gtbocjtnxb.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gttgscfzlw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenlongwang.top/gtgwywbjuq.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtqtwctuqr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangtech.top/gtwfbddlon.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtkrujiqgx.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gtmfpbgqxn.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtgrxibhkn.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtgnjnabyt.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtaleikwwb.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtlpsbhesr.html

[R64] 结束进程
来源：http://hz.sufxvd.cn/gtiqtvzyhv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtyhujlfbn.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtadqmqinn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtnbzucbyw.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtbmzhpgbl.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtmjbddwxm.html

[R67] 生成随机十六进制串
来源：http://hz.fengsongda.top/gtxomfeilx.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtyowcixpn.html

[R68] 计算文件校验值
来源：http://hz.haohaochexian.top/gtqitirhni.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nwbrower.top/gtjfaodvtu.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtdxocxzxj.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtzmwetbvk.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtjsulzucf.html

date +%s;  date -d @1700000000
来源：http://hz.dianchejie.cn/gttwpwbksz.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtvgsyjmod.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gtzvekgjfw.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gtbvlfbvtt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtfuvhlrgp.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtkclfnomi.html

split -l 1000 big.log part_
来源：http://hz.birdmap.top/gtztmuedzs.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtyfiqktgv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shuidangran.top/gtipamtyut.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtqrwmaaii.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtnbqhysiy.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangkeji.top/gtovezhskx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtyltjoqcc.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtbcpxjqtz.html

read -rp "请输入: " ans
来源：http://hz.wangdashe.top/gtbzpdkxvl.html

[R78] 交互式菜单
来源：http://hz.yj20258.top/gtxrnolrmd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtzoucvchu.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtuuczpqnk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtlpzarxcr.html

[R80] 查看脚本执行耗时
来源：http://hz.ybcxt.top/gtqswpddsz.html

time ./run.sh
来源：http://hz.nanxinkj.top/gtbfaavqim.html

================================================================================
来源：http://hz.haohaochexian.top/gtcpvcoqnq.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gtwmtbvaja.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkiffbkdy.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtboobdgqo.html

#include <stdio.h>
来源：http://hz.ehwqpu.com/gtaqxdwqzs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cashguo.top/gtpinqcito.html

[S02] C：变量与格式化输出
来源：http://hz.ywan-chungtsiang.top/gtmhxkzppu.html

int a = 10; printf("%d\n", a);
来源：http://hz.cheryme.top/gtppiplzec.html

[S03] C：读入整数
来源：http://hz.bjfxy.top/gtyxopdaoh.html

int x; scanf("%d", &x);
来源：http://hz.gzhubu.top/gtkqbikiel.html

[S04] C：字符串复制
来源：http://hz.daria6918.cn/gtskrondmn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gttbbmlwca.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtqgnkjrtu.html


<!-- 参考信息 -->
代发 wailian999

[Q36] 左连接
来源：http://hz.gogol.net.cn/gtqhlyowxe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtmlwicefh.html

[Q37] 右连接
来源：http://hz.52xcode.cn/gtavnyfdjx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxinkj.top/gtktzfaxoq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nwbrower.top/gtwrupizje.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.quarkkingdee.top/gtnkywcdui.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtyaxzyqbg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hfpthk.cn/gtlqeoimlp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtipguhaew.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zycfv.cn/gtzgjdnfhc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ywan-chungtsiang.top/gtbjienuek.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gtrqxysnwf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cqqwz.cn/gtlounffye.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pycfn.com/gtpczvvkbg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.havefunace.top/gtpfmyjbtk.html

[Q42] 连接条件附加过滤
来源：http://hz.jinghuilouyu.cn/gtjyyjsmxu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.316326.xyz/gtnhdmzcmf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.andypj.xyz/gtbtekzsqc.html

[Q43] 标量子查询
来源：http://hz.cucudq.cn/gtyzpoqrga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtgbvipyuw.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtckriqwgf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cucudq.cn/gtqsrzpfwe.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtxcpmfvpw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtxmujlcpt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yongpay.top/gtnatkhagh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtqrebzjck.html

[Q47] 与平均值比较
来源：http://hz.yvedp.cn/gtajlehrmw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gthfvjngtd.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigufen.top/gtbwpabrcy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hysaishi.cn/gtyjotltjm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtdbmdcbvj.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtbbnxyboq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenlongwang.top/gtpzojyptg.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtezefqzkj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtzxedmtlp.html

[Q51] 用子查询更新
来源：http://hz.sufxvd.cn/gtjyvmzeof.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fzhhl.top/gtwogzswff.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtsvbqdvki.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtykavnvtb.html

[Q53] 按条件删除
来源：http://hz.meibo888.top/gtporaesxm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gtyyuwkmwy.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtqphwhlok.html

TRUNCATE TABLE logs;
来源：http://hz.redwolf501.top/gtluvmkopq.html

[Q55] 排名（并列占位）
来源：http://hz.nanxuanxn.top/gtdkuhodny.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jianghu66.top/gtkawrcbcg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtoubtaewi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtljkstlwe.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtowbbpnxf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jlsjyb.cn/gtmduccids.html

[Q58] 累计求和
来源：http://hz.chenlongwang.top/gtedxdfgmm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pycfn.com/gtvxxkqdkm.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtajwizvdn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.c1oappe.top/gtweoqqdwa.html

[Q60] 取上一行 / 下一行
来源：http://hz.redwolf501.top/gtxwcyomqw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtqqyqosvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtyiigmwaj.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtksefkvit.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtjsoacoxq.html

[Q62] 分组占比
来源：http://hz.chenjidiqi.icu/gtvzmoyzko.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtiktzvcwr.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtyrhgmgrx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtidlofgyr.html

[Q64] 提交事务
来源：http://hz.kuanghao11.cn/gtbcxuecyn.html

COMMIT;
来源：http://hz.hfpthk.cn/gtnmqvdmfp.html

[Q65] 回滚事务
来源：http://hz.nanxinkj.top/gtdasqjfpo.html

ROLLBACK;
来源：http://hz.dashuyun.cn/gtktlvpvrk.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtnvdfwaqk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.redwolf501.top/gtzuczfasp.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gthjwkgggi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gtbxjatmhc.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtxgvxnelp.html

SAVEPOINT sp1;
来源：http://hz.sxryk.cn/gtthqxtpvs.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtwffmdcfn.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gttbqwzakn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtlngwxgch.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gthnatvocg.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtbkygwmiu.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtoqryawbj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhongyouzk.top/gtitbvnnpq.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtbtmigsov.html

SHOW INDEX FROM users;
来源：http://hz.zhongyouzk.top/gtnlqjvirm.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gtpalsgydm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtunmzglpb.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtkustvzmq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydzc1.top/gtuejvmuwf.html

[Q75] 日期格式化
来源：http://hz.shangyingyoupin.top/gtdddkwuiw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.svipenyu.cn/gtvgzogjgv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.svipenyu.cn/gtgsakhffz.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtdkhqvtvh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtoghzalfd.html

[Q77] 时间加减
来源：http://hz.jinqigfzy.top/gtgreymlmk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtukbbwlog.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gthidnadeu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtpgcylhxw.html

[Q79] 字符串拼接
来源：http://hz.yvedp.cn/gttttlefoh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gticqrtxix.html

[Q80] 字符串截取
来源：http://hz.jinghuilouyu.cn/gtnnyfshst.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.c1oappe.top/gtoylzzird.html

[Q81] 字符串替换
来源：http://hz.snrcjt.cn/gtepkhpght.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtqpnfjbiq.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gthhzdwjrx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pycfn.com/gtygavypry.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtqbbqlpcs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtyycrtgyy.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtgljuavqa.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtnicdaqua.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtnymodwvu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hfpthk.cn/gtworboxco.html

[Q86] 读取 JSON 字段
来源：http://hz.yongpay.top/gtzeloffxe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gtrxgizgww.html

[Q87] JSON 字段做条件
来源：http://hz.gotoacloud.top/gtqdjxzgar.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenjidiqi.icu/gtxntmaiad.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtjgxrcthk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtoqzqojpi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtcpbwddyr.html

[Q89] 判断表是否存在
来源：http://hz.zdqjudy.top/gtallkriyu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtfwgtvxsb.html

[Q90] 生成序号列
来源：http://hz.xuetiantiany.cn/gtecfaikzz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtczfgjtpj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxotzyync.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gtwgvsadro.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdtqafjxc.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtxvigxpex.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtlolndvzm.html

set -euo pipefail
来源：http://hz.yj20258888.top/gtfdgbuzrh.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gtojsjrrpj.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gttlanflzj.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtwhmkfclb.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtxerjlhqy.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtrkinwrxh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gtqgtfvlve.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtutjvqpos.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtiovkftqx.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtfmqbwseq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtmsnhoxxl.html

[R07] if 判断文件
来源：http://hz.zhijiandao.cn/gtxcgnivhv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtomgdisph.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtbtflmsnj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtkxsokvhh.html

[R09] 字符串比较
来源：http://hz.gaohongyu789.top/gtlbvlfrwc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgufenzy.top/gtkuzgcyvr.html

[R10] 正则匹配
来源：http://hz.yvedp.cn/gtqogubsvv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jyoumei.cn/gtggnaefqc.html

[R11] case 多分支
来源：http://hz.snrcjt.cn/gtykoaqyql.html

case "$1" in
来源：http://hz.gotoacloud.top/gtgzuajpqx.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtgwvcbdfs.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtfdujvyks.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtjvwiirrh.html

esac
来源：http://hz.andypj.xyz/gtjkfoatmd.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtxamtsexi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guannengcc.top/gtakkgpzpf.html

[R13] for 计数循环
来源：http://hz.gogol.net.cn/gtjsukgiay.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtkvflxgmo.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtditpjfkw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtwnxwlldt.html

[R15] while 逐行读文件
来源：http://hz.9152youxi.cn/gttybeihai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtclavrlge.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtbukjjkmn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtjnlngvco.html

[R17] 数组定义与取值
来源：http://hz.zhoulong.xyz/gtmzrwymei.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.redwolf501.top/gttlmjjmxf.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtemcjwmkh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtxnrhrmzh.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtclemvgdx.html

echo "${#arr[@]}"
来源：http://hz.cashguo.top/gtzbwjxjqv.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtkntamrnw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sxryk.cn/gtvzcatvdm.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtwypwusfu.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtqklhqmtv.html

[R22] 截取子串
来源：http://hz.hnqzz.top/gtykhtubag.html

echo "${s:0:5}"
来源：http://hz.yongpay.top/gthvdiourx.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtciinwxnt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.redwolf501.top/gtayxzrrlp.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtiixdqknp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gthlqbgqih.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtrlkouajb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtbwbjudkg.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtrndlfhek.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gteqcnizwq.html

[R27] 算术展开
来源：http://hz.hnxiangtu.top/gtekapchge.html

echo $((1 + 2 * 3))
来源：http://hz.zhongyouzk.top/gthiodooqo.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtznezrjat.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtohfagsaj.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gthxwbbkto.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuxming.cn/gtyxbmldiy.html

[R30] 函数返回状态码
来源：http://hz.cheryme.top/gtvxslaxxz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zycfv.cn/gtselwvdku.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gthgyeiaya.html

f() { local x=1; echo "$x"; }
来源：http://hz.redwolf501.top/gtpxqvdlxj.html

[R32] 参数个数校验
来源：http://hz.cucudq.cn/gtbjoxvdir.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtvdixnvzk.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtucqavkby.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtrzrydakp.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtxavbietc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtzyygfetu.html

[R35] 后台执行并等待
来源：http://hz.yueranfly.top/gtfqqevlqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gaohongyu789.top/gtoxbtskno.html

[R36] 并发执行多个任务
来源：http://hz.yanxiufei.cn/gtlrmsafxr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtiwtvzpqq.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtoatlnfju.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtobkndglv.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gtclsvoylz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cdnleiting.top/gtdxvbqzas.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtikpwfimt.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtemoceqqa.html

[R40] 追加写日志
来源：http://hz.yangfankeji.com/gthqwysgrx.html

echo "log" >> out.log
来源：http://hz.fengsongda.top/gtsgtnjbpy.html

[R41] 丢弃输出
来源：http://hz.cheryme.top/gtcfujxrsc.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gteilvohse.html

[R42] 输入重定向
来源：http://hz.shuidangran.top/gtouclpzuu.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtfvpkmxue.html

[R43] 按名字查找文件
来源：http://hz.quarkkingdee.top/gtwhhoglwa.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtlfbqxahl.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtmsktehgf.html

find . -mtime -7 -type f
来源：http://hz.sufxvd.cn/gtprjakivc.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtpglxertu.html

find . -name "*.tmp" -delete
来源：http://hz.xziqi.cn/gtsfkpdiha.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtrdfbsols.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ehwqpu.com/gtcrgxxnmu.html

[R47] sed 单行替换
来源：http://hz.meibo888.top/gtkhwfdpss.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtvptsgfmt.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtcnbpxcfs.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtugbggeuq.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtvntzksjc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtqnxsbgig.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gtneemwlsm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtaypsbqzx.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gthcxrdleo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gtkqctmcbp.html

[R52] 统计行数
来源：http://hz.xuanzx.com/gtwmmxrcwc.html

wc -l a.txt
来源：http://hz.guowangkeji.top/gtngcayghs.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtvuwyujph.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtwumppaya.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtglbawacg.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtihfwhqci.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtxfttffzy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtzpwmzypz.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtvmnvjtfj.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtdcxzlzhn.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtbiuzaxpz.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtnmycyobh.html

[R58] 下载文件
来源：http://hz.316326.xyz/gtoygpawbc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yueranfly.top/gtgkzatjuu.html

[R59] 发 POST JSON
来源：http://hz.jiagoushi.top/gttgtirawp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gthtruszwl.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtvorbvcgj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtqfhlrnwv.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangkeji.top/gtawowkxvs.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtcsdzfvim.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtsgjxlsog.html

du -ah . | sort -rh | head -10
来源：http://hz.yongpay.top/gtcyzvsijp.html

[R63] 内存与进程
来源：http://hz.316326.xyz/gtixmirtuq.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtvnxsgxlf.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtckvjhzie.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtoxdkoszp.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtafwuhjoz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gtakemohch.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gtsrnxmnef.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtxveewhau.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gtobwtrdmm.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtdovhqada.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtubgnuwox.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtapstgxwo.html

[R69] 生成随机密码
来源：http://hz.birdmap.top/gtzkkvuduu.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtnphnvjsc.html

[R70] 时间戳与互转
来源：http://hz.ehwqpu.com/gtjmrglqjx.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtlhwxwubg.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtbeelgdmv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtzegmkkzn.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtyjhppcuu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtipbeggjn.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtefgmfbqz.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtvaoxrnoz.html

[R74] 批量重命名
来源：http://hz.ppjwa.cn/gtijonmbtj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtgqbqiugs.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtgkojclil.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtvbvepktk.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtdvpanvrg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gthczguirc.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtmbhaekjt.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtemuecuob.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gtqebaibil.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnxiangtu.top/gtgyjtyyme.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtqlnlcgst.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gtgptqnmzc.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangkeji.top/gtokvrklod.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtexyjnpxd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlhkdtccn.html

S. C / C++ 专题
来源：http://hz.zycfv.cn/gtlivcmedy.html

================================================================================
来源：http://hz.havefunace.top/gttfwlrcmg.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtorzyawbf.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtgvtrgvns.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtjubrviup.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gtomtxjfcf.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gttqbvrixk.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gthzittcwq.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtisjaaauh.html

[S04] C：字符串复制
来源：http://hz.haohaochexian.top/gtxvlpfsso.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.svipenyu.cn/gtnvjfxfgx.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gtqkiznzea.html


<!-- 参考信息 -->
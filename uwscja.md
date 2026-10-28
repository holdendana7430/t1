代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtlphirgbd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xinyue.icu/gtatjyckrl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtizfcjhpr.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gttealgszc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuetiantiany.cn/gtbweykrhx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gtiackszdr.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtthyeznek.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gthyjxbgdo.html

[Q44] IN 子查询
来源：http://hz.shuidangran.top/gtmbuvcgkq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj202588.top/gtgbovhtwi.html

[Q45] EXISTS 判断存在
来源：http://hz.chenjidiqi.icu/gtkexoxeit.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtiujwyvfl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydjk.org.cn/gtgifqpodn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtjphotgsu.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtiponkrwj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.haohaochexian.top/gtiuhnjhdq.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtjmspeyux.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gtmyqwqjkc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gaohongyu789.top/gtbambzpov.html

[Q49] 更新单行
来源：http://hz.chenjidiqi.icu/gtegszcdtu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuxming.cn/gtafytxqfp.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtheniexhf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gtsgiwjuvy.html

[Q51] 用子查询更新
来源：http://hz.yuxming.cn/gtgyqesuil.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtbaqzpyxx.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtsigzgbsg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gtlcfpscyq.html

[Q53] 按条件删除
来源：http://hz.gotoacloud.top/gtcmwnzuat.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtwxzqbwdi.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtwcwiagxv.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtduknbfgu.html

[Q55] 排名（并列占位）
来源：http://hz.nwbrower.top/gtvcpwjsvs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gteufmayyv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhiwuduotai.top/gthnrskboh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgfzy.top/gtfrzcrnsl.html

[Q57] 行号
来源：http://hz.cheryme.top/gtcgocyewz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guowangkeji.top/gtoqhjpbmb.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtwsfmrysg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtnxuzwsht.html

[Q59] 分组内累计
来源：http://hz.pycfn.com/gtcfqlzzbl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtlzedvvvs.html

[Q60] 取上一行 / 下一行
来源：http://hz.xziqi.cn/gtneiizrwx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtgwiezgpt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtloanpxdj.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtcftspmpl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhixingplan.top/gtcveimrgy.html

[Q62] 分组占比
来源：http://hz.tianlin.xyz/gtnyyfffse.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtrlhdkxxj.html

[Q63] 开启事务
来源：http://hz.pycfn.com/gturgpdtzf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtfpbdttkx.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtuunbgouh.html

COMMIT;
来源：http://hz.shanyushiyangtech.top/gthmggaynd.html

[Q65] 回滚事务
来源：http://hz.nwbrower.top/gtinojngkz.html

ROLLBACK;
来源：http://hz.xuetiantiany.cn/gtqsdqkvmd.html

[Q66] 行锁查询
来源：http://hz.c1oappe.top/gtpkhjeone.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtfatmeeaa.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtzfbcedtm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigufen.top/gtceglgsgz.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtsrbmvlvx.html

SAVEPOINT sp1;
来源：http://hz.andypj.xyz/gttvbdtbfs.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtugfzmfyd.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtohlhnpez.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gtewwakrmk.html

[Q70] 更新统计信息
来源：http://hz.yuxming.cn/gtaguentwh.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gthmgqfemz.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gttwsnqrls.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yangfankeji.com/gtfodkrbkf.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtziuwurvk.html

SHOW INDEX FROM users;
来源：http://hz.havefunace.top/gtmmmmmfim.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtyrtajdhn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aizwys.cn/gtksaylcwe.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtuegspfjt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gthfqsblqx.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtmqvrcdux.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtewvxaimd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zdqjudy.top/gtyysnunbx.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtojvtlaio.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gtzyxkxnkq.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtxaucjuhb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtlwauqvyp.html

[Q78] 当前时间
来源：http://hz.iojbl.cn/gtgoejurjt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtjeplxkhi.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtcvowucov.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtbegxhomo.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtihmctdqn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtxjhiqedx.html

[Q81] 字符串替换
来源：http://hz.xinyue.icu/gtamoinbcn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gtksqoqhyo.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gtbxwnyxnb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gtucepjtep.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtjditjkph.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnxiangtu.top/gtbyfdkitk.html

[Q84] 去除首尾空格
来源：http://hz.tanke756.top/gtmcbujlxm.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtxooiluvt.html

[Q85] 数值取整
来源：http://hz.jqgfzy.top/gticjraalc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtjyroqyaj.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtfacxkact.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtrhfgwcxt.html

[Q87] JSON 字段做条件
来源：http://hz.cashguo.top/gtmwbuogvr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cucudq.cn/gtkstgmlvt.html

[Q88] 行转列（条件聚合）
来源：http://hz.fzhhl.top/gtmecbhiec.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jyoumei.cn/gthlvwetkj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgfzy.top/gtehnytsam.html

[Q89] 判断表是否存在
来源：http://hz.chenlongwang.top/gtgcgrxmfd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhiwuduotai.top/gtmnlneloa.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtbkthcenw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gtmlzwvmqz.html

================================================================================
来源：http://hz.yueranfly.top/gtgilxsdvn.html

R. Bash 专题
来源：http://hz.xylfe.cn/gthtopimmg.html

================================================================================
来源：http://hz.zycfv.cn/gtkcwvrirw.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gtmjbigfwk.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gteoxzfemf.html

set -euo pipefail
来源：http://hz.hywenlv.cn/gtkyxsknhe.html

[R02] 变量赋值与使用
来源：http://hz.yonumen.top/gtavntojot.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtewkepwui.html

[R03] 只读变量
来源：http://hz.hfpthk.cn/gtlkcenirh.html

readonly PI=3.14
来源：http://hz.hnqzz.top/gtbkrhclnp.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtzavhqluo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhiwuduotai.top/gtxnxsywde.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtsahxkpjb.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtmdccrcfo.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtniqutotc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtscaftoxl.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtsozvfutt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtkmfbtpde.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gttyhzssug.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtgouphsur.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gtbvnqogyb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtwjuehmtv.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtrgrlizqn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtawykccdt.html

[R11] case 多分支
来源：http://hz.c1oappe.top/gtjewxjgai.html

case "$1" in
来源：http://hz.tianlin.xyz/gttwcjieew.html

start) echo "启动" ;;
来源：http://hz.xingfuxueyuan.xyz/gteqwcehcn.html

stop)  echo "停止" ;;
来源：http://hz.ehwqpu.com/gtdltjinzg.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gteufnwgvx.html

esac
来源：http://hz.meibo888.top/gtklnqbwdx.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gthzhzujdv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuetiantiany.cn/gtvdppmcai.html

[R13] for 计数循环
来源：http://hz.tian-w.cn/gtkwjcbhfx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hysaishi.cn/gtzjjlepkv.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gttqiqtkyn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gotoacloud.top/gtodtxzlkk.html

[R15] while 逐行读文件
来源：http://hz.mhx1999.top/gtewekpwya.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.pycfn.com/gtffuvfaco.html

[R16] until 等待条件
来源：http://hz.hammf.cn/gtiybsyuia.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtrtcobssf.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtqfsecpzh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtcscdjiel.html

[R18] 遍历数组
来源：http://hz.jinqigufen.top/gtfflzhckh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtgewyazdw.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtaupplsbn.html

echo "${#arr[@]}"
来源：http://hz.feifeiyinyue.top/gtbprjelmx.html

[R20] 关联数组（字典）
来源：http://hz.yvedp.cn/gtxfkqohxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtclyfhwwg.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gtuptjvpvl.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtygkghave.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtfatqvbip.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtucpgmoos.html

[R23] 字符串替换
来源：http://hz.ivvv.top/gtuwqvzxiu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtoefrpqxt.html

[R24] 大小写转换
来源：http://hz.zhijiandao.cn/gtcprphjpv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gtsaaqsssg.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtpyvqwrdh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtaojcuqmt.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtqsbxokqx.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtleacpapg.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtgrssklcw.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtzgjtohqy.html

[R28] 浮点运算
来源：http://hz.birdmap.top/gtrlefqymy.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtdtxnhbdg.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtrerzxobr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxuanxn.top/gttllzjlbg.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtqxxsyahr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtirksiaug.html

[R31] 局部变量
来源：http://hz.ydzc1.top/gtuygefero.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtqymvwegv.html

[R32] 参数个数校验
来源：http://hz.yuxming.cn/gtsffrzbwl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtntotbyan.html

[R33] 捕获错误并提示行号
来源：http://hz.sysykeji.top/gtasbcqxwd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtwzdfiqwf.html

[R34] 退出时清理
来源：http://hz.xuetiantiany.cn/gtzucisrqy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtsqdqkomc.html

[R35] 后台执行并等待
来源：http://hz.52xcode.cn/gtfbptjbts.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtfsxmdaiz.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtndsuqaur.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtjvactymh.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtqxwbemkz.html

files=$(ls -1)
来源：http://hz.yangfankeji.com/gtputadvlq.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtsrhourov.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtmwkwapaz.html

[R39] 重定向标准输出与错误
来源：http://hz.xinyue.icu/gtbvvkxrkn.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtengczoap.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtkyebbujx.html

echo "log" >> out.log
来源：http://hz.xingfuxueyuan.xyz/gttwjrcdat.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtuqzdoicu.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gtlhfsxupf.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtkpteiiya.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtkejqwqos.html

[R43] 按名字查找文件
来源：http://hz.jlsjyb.cn/gtebmocppo.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtdrwhmrri.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtmldmopga.html

find . -mtime -7 -type f
来源：http://hz.chenlongwang.top/gtjwklxnhn.html

[R45] 批量删除
来源：http://hz.zhiwuduotai.top/gttifhgnoi.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtmdurbsdz.html

[R46] 递归替换文件内容
来源：http://hz.yongpay.top/gtoswsfmjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtexbqshch.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gttsjjijry.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtpvokbbyg.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtdtveadlp.html

awk '{print $1, $3}' a.txt
来源：http://hz.vqdsnc.cn/gtzklvnbzq.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtprmomkcq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtgnosiivj.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtoximflob.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtbdrsthcg.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gthbleobem.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuanzx.com/gtfvwbfbzb.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtycjksbwr.html

wc -l a.txt
来源：http://hz.fengsongda.top/gtenrutxtp.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxuanxn.top/gtixfirptv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtdgspgtnq.html

[R54] 比较两个文件
来源：http://hz.iojbl.cn/gtoxcxnhcn.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtlvxnpjjb.html

[R55] 压缩与解压
来源：http://hz.ppjwa.cn/gtysbqhutq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtokqqenyz.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtartznazc.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gttonpovxo.html

[R57] 远程执行命令
来源：http://hz.guowangkeji.top/gtthdqhdiv.html

ssh user@host 'uptime'
来源：http://hz.shuidangran.top/gtnxuchofc.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtlmfdjdwl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yueranfly.top/gtghkscdzh.html

[R59] 发 POST JSON
来源：http://hz.yangfankeji.com/gtbxmlwgtp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtfgbdtfkg.html

[R60] 只看 HTTP 状态码
来源：http://hz.jianghu66.top/gtooixtwkb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtydirifbl.html

[R61] 磁盘占用
来源：http://hz.zhoulong.xyz/gtiawrkxhd.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtnzxaxlyp.html

[R62] 找最占空间的文件
来源：http://hz.jlsjyb.cn/gtmvdocyoi.html

du -ah . | sort -rh | head -10
来源：http://hz.yj202588.top/gtqxifiqjl.html

[R63] 内存与进程
来源：http://hz.yj202588.top/gtzkrexjfi.html

free -h;  ps aux | grep nginx
来源：http://hz.52xcode.cn/gtzwziwhck.html

[R64] 结束进程
来源：http://hz.nwbrower.top/gtmohkakth.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtwqqtslwd.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtcdvqyeia.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtqjlfrflv.html

[R66] 定时任务
来源：http://hz.daria6918.cn/gtnhvuovhz.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gttuihxjuv.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtwenwbjlf.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtealrlljo.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gttvaedcad.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtsrrpcjlz.html

[R69] 生成随机密码
来源：http://hz.xylfe.cn/gtgvaioyus.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtbjpsgkir.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtnnygxwxs.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtxbcsbfog.html

[R71] 日期格式化
来源：http://hz.ydjk.org.cn/gtobtqbowf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gtkjkhogvg.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtsfrestbx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtofadbqzi.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtxtproaqf.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gthttfqdzx.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtomrtkvek.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtrtzkards.html

[R75] 导出环境变量
来源：http://hz.xylfe.cn/gtvhfnuldi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtbkebtnjy.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtseycvtyh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtkgdgwlpy.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtimtkdhaj.html

read -rp "请输入: " ans
来源：http://hz.vqdsnc.cn/gtxgrngcke.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gtijwogmjz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnxiangtu.top/gtqscfdqbq.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtjebhgnvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nwbrower.top/gttsmwgmyn.html

[R80] 查看脚本执行耗时
来源：http://hz.wangshuangyany.cn/gtadrwsqpz.html

time ./run.sh
来源：http://hz.shuidangran.top/gtjbypjufd.html

================================================================================
来源：http://hz.wangdashe.top/gttvuwupst.html

S. C / C++ 专题
来源：http://hz.jinqigufen.top/gttufnjocx.html

================================================================================
来源：http://hz.redwolf501.top/gtmbiyoemp.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtsxmkjjpr.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtucrvgohv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtpniwyxry.html

[S02] C：变量与格式化输出
来源：http://hz.yongpay.top/gtfotjmtpt.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtbetpcqgf.html

[S03] C：读入整数
来源：http://hz.yangfankeji.com/gtbeixmmco.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gttpmwmbho.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtubsdfftv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.mhx1999.top/gtmhyydnjm.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtcafiivlu.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gttoimxfqy.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtkuwvyvbl.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtassasuxo.html

[S07] C：数组遍历求和
来源：http://hz.smart0.xyz/gtizohukav.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtuohchqke.html

[S08] C：动态内存分配与释放
来源：http://hz.fzhhl.top/gtclhnhyvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gtbrfsyvhr.html

[S09] C：结构体定义与初始化
来源：http://hz.hfpthk.cn/gteclwetej.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtveixdisa.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtxbbiytgi.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtacfkytxq.html

[S11] C：逐行读文件
来源：http://hz.jqgufenzy.top/gthxhavhdq.html


<!-- 参考信息 -->
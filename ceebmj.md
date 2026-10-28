代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.9152youxi.cn/gtdkxoijou.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtqjbkbpzq.html

[Q43] 标量子查询
来源：http://hz.yj20258888.top/gtiqwatwgk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gthbbbmexu.html

[Q44] IN 子查询
来源：http://hz.fengsongda.top/gtuqqbefzy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtrsiynjnq.html

[Q45] EXISTS 判断存在
来源：http://hz.yanxiufei.cn/gtscduuaeh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gthnvrammt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtzawjhtrg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtqxuxpgcl.html

[Q47] 与平均值比较
来源：http://hz.birdmap.top/gtxgknkvfy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtwousyuoa.html

[Q48] CTE 公用表表达式
来源：http://hz.hnqzz.top/gtgtlvifys.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cashguo.top/gthwkjxwrx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtmpzlurvq.html

[Q49] 更新单行
来源：http://hz.shangyingyoupin.top/gtwvghgfed.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtdqrqgeos.html

[Q50] 批量更新
来源：http://hz.dianchejie.cn/gtoxpqadpx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuxming.cn/gtxwdivzbq.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gttxipzgfa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ppjwa.cn/gtjncaxtyw.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtvbgtlucx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtkravvwoo.html

[Q53] 按条件删除
来源：http://hz.wangdashe.top/gtldiljfne.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtspzpwywl.html

[Q54] 清空表
来源：http://hz.cashguo.top/gteklwnuqk.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gtqdmnxquc.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtlgojymnp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtyxxtausa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtkipxzqwr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tian-w.cn/gtpnpzvbxr.html

[Q57] 行号
来源：http://hz.zycfv.cn/gtaygtahsm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuanzhike.top/gtehhbezjh.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtootcdkvg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jiagoushi.top/gtexurtgql.html

[Q59] 分组内累计
来源：http://hz.wangshuangyany.cn/gthotpxqko.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xinyue.icu/gtjixgexrm.html

[Q60] 取上一行 / 下一行
来源：http://hz.iojbl.cn/gtfvkvkrxu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtjeltftwb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtxdjhhepa.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtorfaswse.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jlsjyb.cn/gtbiykqgrh.html

[Q62] 分组占比
来源：http://hz.gaohongyu789.top/gtccndnhrz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtnarqdxzq.html

[Q63] 开启事务
来源：http://hz.zhaomingkeji.xyz/gtaavsogeb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yonumen.top/gtzlivarfo.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtbulpgnnp.html

COMMIT;
来源：http://hz.shanyushiyangtech.top/gtigbfpgdi.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtgoxkwzmb.html

ROLLBACK;
来源：http://hz.yuxming.cn/gthmblpnmh.html

[Q66] 行锁查询
来源：http://hz.tian-w.cn/gtmcvemmuk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gtqbcxsxmk.html

[Q67] 设置隔离级别
来源：http://hz.hysaishi.cn/gtpewttpad.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.haohaochexian.top/gtoxcdezia.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtokbqubte.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gtvwfokwfm.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtarqscrlx.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtxakmmfey.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gtpvmhehzb.html

[Q70] 更新统计信息
来源：http://hz.cashguo.top/gttojzojpz.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtwtkxaxuy.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gtidircdzl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtpnptuxxy.html

[Q72] 查看索引
来源：http://hz.tanke756.top/gtiahnqulx.html

SHOW INDEX FROM users;
来源：http://hz.guowangkeji.top/gtjpsifdkv.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gtiugxotfy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtmtfpfppi.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gtgjgwirgu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtbhyvwmys.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gtghbuzwxb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtoxjcvzns.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daxiang520.top/gtgrzkfsbh.html

[Q76] 按天统计
来源：http://hz.316326.xyz/gttmkookdj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sysykeji.top/gtocmdctbq.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gttsbfsyxn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.bjfxy.top/gtuszlggoi.html

[Q78] 当前时间
来源：http://hz.zhengqikj.top/gtehccyhqi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigfzy.top/gtktvwhbuv.html

[Q79] 字符串拼接
来源：http://hz.ehwqpu.com/gtxnebfucn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtbkdyfmrp.html

[Q80] 字符串截取
来源：http://hz.quarkkingdee.top/gthzucpudb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hongshengwenyu.top/gtmehatjho.html

[Q81] 字符串替换
来源：http://hz.chenlongwang.top/gtnqjgkkah.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtoimbvpxb.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gtktpcsveo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gttolkpphp.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtkqhawgpi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.9152youxi.cn/gtzlxubawx.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtyxgokuzp.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtdeqgjwnj.html

[Q85] 数值取整
来源：http://hz.yangfankeji.com/gtjsxkmlsz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhiwuduotai.top/gtobwridgm.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtnjfpzldj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtqmonysku.html

[Q87] JSON 字段做条件
来源：http://hz.hywenlv.cn/gtjyemtddv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nwbrower.top/gtcbfkmurb.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtrhwvkxdc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shuidangran.top/gtebdjipnk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.haohaochexian.top/gtcbkypjkj.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtpadpvfst.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xylfe.cn/gtpdkccnfi.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtrwnvpcdw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtkhnfapvw.html

================================================================================
来源：http://hz.sufxvd.cn/gttlumlwnt.html

R. Bash 专题
来源：http://hz.yuxming.cn/gteqiqqggs.html

================================================================================
来源：http://hz.sysykeji.top/gtlvxxingz.html

[R01] shebang 与严格模式
来源：http://hz.hywenlv.cn/gtmmontjex.html

#!/usr/bin/env bash
来源：http://hz.tianlin.xyz/gtzxwahqjb.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gtxiscmrjg.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtrpfeigbp.html

name="Tom"; echo "$name"
来源：http://hz.bjfxy.top/gthajiposu.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtrkngrjkh.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtxvkfaeyi.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtcaspiken.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtqqfehlle.html

[R05] 参数默认值
来源：http://hz.xuetiantiany.cn/gthsmtemlq.html

name="${1:-default}"
来源：http://hz.0kj1m.cn/gtpwbqpqij.html

[R06] 判断命令是否存在
来源：http://hz.aizwys.cn/gttyaqmuhf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtlkvmhmbp.html

[R07] if 判断文件
来源：http://hz.52xcode.cn/gtolsxkruc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydjk.org.cn/gtatuvrdtn.html

[R08] 数值比较
来源：http://hz.haohaochexian.top/gtggxodxux.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtecxyfnfi.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gthqkwxxkj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtfoxvlmml.html

[R10] 正则匹配
来源：http://hz.iojbl.cn/gtlzforkbn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtqyjqizww.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gttrrbwslt.html

case "$1" in
来源：http://hz.quarkkingdee.top/gtokmiqnxu.html

start) echo "启动" ;;
来源：http://hz.9152youxi.cn/gtzliwirwr.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtlfvdrffk.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtyrrszsxp.html

esac
来源：http://hz.yuanzhike.top/gtsypowxax.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtxlcosfwx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtefurefvw.html

[R13] for 计数循环
来源：http://hz.tanke756.top/gtsyzevinm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtxxlttuem.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gtdlfastif.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtnybbjjhr.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtwarqlytk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtcnpcqjro.html

[R16] until 等待条件
来源：http://hz.yangfankeji.com/gtijfbjjwo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtvxderfig.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtrfdnzlaa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.52xcode.cn/gthauihtyw.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtfbvkugkn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydzc1.top/gtqstjpkcx.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtcwwgqmim.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtrlkhbggf.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gttsvzqihg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.0kj1m.cn/gtocgiupcl.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtafylwszt.html

echo "${#s}"
来源：http://hz.gaohongyu789.top/gtrjeqkslx.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtrqkjyuyd.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtpsidyexa.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtbdfiilhp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtpcczqsob.html

[R24] 大小写转换
来源：http://hz.zhijiandao.cn/gtcalzngii.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aizwys.cn/gtwkpyxbqm.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangdashe.top/gtexcekdwv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gtfdihlqqs.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtxmmwgcyl.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258888.top/gtlaqpkash.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtfjcvedtt.html

echo $((1 + 2 * 3))
来源：http://hz.gogol.net.cn/gthtnbsylt.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtmfgwjtcc.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtwoomtuec.html

[R29] 定义函数
来源：http://hz.pengpengdd.cyou/gtlkcebeog.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtfgdhmhrw.html

[R30] 函数返回状态码
来源：http://hz.jqgfzy.top/gtzkhngrdv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtcpdbdols.html

[R31] 局部变量
来源：http://hz.zhoulong.xyz/gtbgsvouxe.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258888.top/gtagtcfdhi.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtxzhltrab.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtkcykzzmc.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtfulwpykv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangdashe.top/gtwjaaruab.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtirtbzipm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtkvolibyd.html

[R35] 后台执行并等待
来源：http://hz.52xcode.cn/gtofqcurna.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pycfn.com/gtmwfhfdlo.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtnjqyltdb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtumyiovfk.html

[R37] 把输出赋给变量
来源：http://hz.zhiwuduotai.top/gtffekidgx.html

files=$(ls -1)
来源：http://hz.zhengqikj.top/gtxqqrllsk.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtauncsqxw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.vqdsnc.cn/gtqphxkpuu.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gteldvyqfy.html

cmd > out.log 2>&1
来源：http://hz.snrcjt.cn/gtrpggtbyc.html

[R40] 追加写日志
来源：http://hz.jianghu66.top/gtaejekiyc.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gttrolwgwj.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtudrbmmps.html

cmd >/dev/null 2>&1
来源：http://hz.gaohongyu789.top/gtgnnyjklk.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtrgctrkzm.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtsatshwmi.html

[R43] 按名字查找文件
来源：http://hz.fengsongda.top/gtszklwnhs.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtvgbkvdit.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtzsqygfyg.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtivhytund.html

[R45] 批量删除
来源：http://hz.pycfn.com/gtcppxolvu.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtsbxabeiw.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtmeimpgnw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.haohaochexian.top/gtasfncyrm.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtiqopaoat.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.52xcode.cn/gtvokkwimm.html

[R48] awk 取指定列
来源：http://hz.aibaodan.cn/gtncwyzwjs.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtmhkdezwq.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtozsnzubi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtahszbimq.html

[R50] awk 求和
来源：http://hz.yanxiufei.cn/gtwykzitpg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnxiangtu.top/gtptqdvurm.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtjfozaars.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhaomingkeji.xyz/gtkwiqbitm.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtfhyrydaj.html

wc -l a.txt
来源：http://hz.cheryme.top/gtbhkjmhbr.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtbkyorgkw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtzyugewkl.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtlbvhxuln.html

diff a.txt b.txt
来源：http://hz.cheryme.top/gtamrxnejv.html

[R55] 压缩与解压
来源：http://hz.tianlin.xyz/gtyiibjdva.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtjvmcllyv.html

[R56] 远程拷贝
来源：http://hz.guannengcc.top/gtkxyouwml.html

scp file user@host:/path/
来源：http://hz.shangyingyoupin.top/gtakvkyiag.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtkvgdjwrl.html

ssh user@host 'uptime'
来源：http://hz.jinyuanbaomall.cn/gtrxtkdrcn.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gttuqjybej.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guannengcc.top/gtnjvflzoe.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gtutgriglk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gtilzulttl.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtxgbjzumg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.iojbl.cn/gttcvkfzrv.html

[R61] 磁盘占用
来源：http://hz.yonumen.top/gtoadrivda.html

df -h;  du -sh *
来源：http://hz.52xcode.cn/gtmmzanoue.html

[R62] 找最占空间的文件
来源：http://hz.zhaomingkeji.xyz/gtjtwdbxzo.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gthekiepal.html

[R63] 内存与进程
来源：http://hz.ydzc1.top/gtkwvezdmr.html

free -h;  ps aux | grep nginx
来源：http://hz.yanxiufei.cn/gtokyichub.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtlyxqukvt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtofepsvcx.html

[R65] 查看端口占用
来源：http://hz.gaohongyu789.top/gtodftdwjw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dashuyun.cn/gtrsjsnhzj.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtphhnmslc.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtqxkqiauk.html

[R67] 生成随机十六进制串
来源：http://hz.zhengqikj.top/gtrnjiitgk.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtlkoyyocq.html

[R68] 计算文件校验值
来源：http://hz.yongpay.top/gtuvvlmycp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gtpydxuluv.html

[R69] 生成随机密码
来源：http://hz.wangdashe.top/gtzwfhjrfl.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gthpiflmkc.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtyjpizpfc.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtidgtmxfm.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtzdzvwdci.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtnalqvuzz.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtblbejlml.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtjlisyvgu.html

[R73] 分割大日志
来源：http://hz.pengpengdd.cyou/gtpgyqmdef.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtdijymlei.html

[R74] 批量重命名
来源：http://hz.cashguo.top/gtbljaoera.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtcpqgxmxp.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gthdthlotn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtvqyeeuoa.html

[R76] 使用临时文件
来源：http://hz.zhijiandao.cn/gtvgnbhmeh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtkpnvmshz.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtzfiquznh.html

read -rp "请输入: " ans
来源：http://hz.jyoumei.cn/gtkwpurobg.html

[R78] 交互式菜单
来源：http://hz.birdmap.top/gtnpeunwxq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtuaqpqizl.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtooyybnxl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtlhbpvuqt.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gtdvcwonnz.html

time ./run.sh
来源：http://hz.dashuyun.cn/gtvacjjmmy.html

================================================================================
来源：http://hz.aizwys.cn/gtopkvwipy.html

S. C / C++ 专题
来源：http://hz.jianghu66.top/gtfprxewms.html

================================================================================
来源：http://hz.cucudq.cn/gttkxbghve.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtnflviniv.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtndybtqyg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtxiuxfwfj.html

[S02] C：变量与格式化输出
来源：http://hz.zhijiandao.cn/gtrsankjfo.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinyuanbaomall.cn/gtxknwthno.html

[S03] C：读入整数
来源：http://hz.ybcxt.top/gtqowyepnl.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gticvetecz.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtiagehtfb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangkeji.top/gtbziqmfuo.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gteryvnbgo.html

strlen(s)
来源：http://hz.yuanzhike.top/gtfujdmmau.html

[S06] C：字符串比较
来源：http://hz.haohaochexian.top/gtdcfciogy.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtrfbxrlhe.html

[S07] C：数组遍历求和
来源：http://hz.tian-w.cn/gtijftlbyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhaomingkeji.xyz/gtpyjtdtcm.html

[S08] C：动态内存分配与释放
来源：http://hz.dianchejie.cn/gtjkgdgrud.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtccyplnnu.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtznpkyqdw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gtmgwqrhkq.html

[S10] C：指针与解引用
来源：http://hz.jinyuanbaomall.cn/gtccrtcrvn.html

int *p = &a;  *p = 5;
来源：http://hz.xingfuxueyuan.xyz/gtypeloyxr.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gtlqmhuxqw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gttzaeojpy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gttvuykyuw.html

fclose(f);
来源：http://hz.cqqwz.cn/gtyneybods.html

[S12] C：写文件
来源：http://hz.aizwys.cn/gtuzctnapp.html


<!-- 参考信息 -->
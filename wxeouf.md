代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenlongwang.top/gtviiqrwxh.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtxsghjbxj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gtpyrxmhlk.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtgrfjohhh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jlsjyb.cn/gtmweotocc.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gteckyqqtl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtcfqljumh.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtyxdldxqj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.quarkkingdee.top/gtwnhwqcgl.html

[Q54] 清空表
来源：http://hz.aizwys.cn/gtpacwnadi.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtkaegmxwt.html

[Q55] 排名（并列占位）
来源：http://hz.yj202588.top/gtmvkxzfvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtituswzwn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.mhx1999.top/gtvtcotpuh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tanke756.top/gtroukeriu.html

[Q57] 行号
来源：http://hz.daxiang520.top/gthterfmfk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydjk.org.cn/gtontfzmqb.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtdjipnswn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydzc1.top/gtpfvywjfq.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtfylkmklu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtrjoopgup.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258.top/gthscsfusm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtgaeptnkg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gttomqfgdi.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gtfwyuxojn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtejehjygd.html

[Q62] 分组占比
来源：http://hz.shuidangran.top/gtuvtumjwe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtzclssioy.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtedqqcldy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhoulong.xyz/gtyyigkkef.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gttjafqvek.html

COMMIT;
来源：http://hz.jinqigufen.top/gtpniyfucl.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gtsianodyw.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtpfwaamww.html

[Q66] 行锁查询
来源：http://hz.xylfe.cn/gtzmoubodk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gtydehzkqv.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtxwjqfyio.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigfzy.top/gtjftdngqe.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtuzqkgvyf.html

SAVEPOINT sp1;
来源：http://hz.fzhhl.top/gtxycsyayn.html

ROLLBACK TO sp1;
来源：http://hz.snrcjt.cn/gtdgdutwgg.html

[Q69] 查看执行计划
来源：http://hz.zycfv.cn/gtrcpopbjf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.svipenyu.cn/gthbnfdcnw.html

[Q70] 更新统计信息
来源：http://hz.tianlin.xyz/gtwglubrno.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtegudyacw.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtecezyncd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gttsdjnhfs.html

[Q72] 查看索引
来源：http://hz.jqgfzy.top/gtuiavahjn.html

SHOW INDEX FROM users;
来源：http://hz.yj202588.top/gtycbhiafc.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gtozmaxuii.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtlplsblrj.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtetmtysvy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtrrnjlkau.html

[Q75] 日期格式化
来源：http://hz.gzhubu.top/gtbopuyyll.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gtnjimoonn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gtxksmfwtk.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gtdngdlooy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtprneefye.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtlkuwsndp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guowangkeji.top/gtqlhrwnku.html

[Q78] 当前时间
来源：http://hz.xuanzx.com/gtcrvnxdan.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zycfv.cn/gtbmhutisv.html

[Q79] 字符串拼接
来源：http://hz.yonumen.top/gtapzjwwsb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ywan-chungtsiang.top/gtvchpcrlv.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtdkezalwy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtjdbvwnds.html

[Q81] 字符串替换
来源：http://hz.pycfn.com/gtxuglrhvz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhiwuduotai.top/gttwttzcnc.html

[Q82] 字符长度与字节长度
来源：http://hz.gaohongyu789.top/gtzcfeejcz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.kuanghao11.cn/gtfekmxuxn.html

[Q83] 大小写转换
来源：http://hz.meibo888.top/gtwxjkuedh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhengqikj.top/gtmbfyoyck.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtpxtftuzh.html

SELECT TRIM(name) FROM users;
来源：http://hz.gzhubu.top/gtcxpilray.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gthkjmqxzi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtvcdkdoea.html

[Q86] 读取 JSON 字段
来源：http://hz.ydzc1.top/gtrrwktewk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtztnwgrhv.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtczfibobn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtfwxodvor.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuetiantiany.cn/gtqxvqdkbp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtpkkgrpbx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtsedhsnsk.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtcjkyehvw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtwayphwiv.html

[Q90] 生成序号列
来源：http://hz.ybcxt.top/gtcxowfaaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtgpejnygo.html

================================================================================
来源：http://hz.ydzc1.top/gtpaaijuvq.html

R. Bash 专题
来源：http://hz.shanyushiyangtech.top/gtwkpfqfuo.html

================================================================================
来源：http://hz.52xcode.cn/gtsgdkxnlw.html

[R01] shebang 与严格模式
来源：http://hz.chenjidiqi.icu/gtetgmlzsq.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtdfmvboqz.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtsolzjqyj.html

[R02] 变量赋值与使用
来源：http://hz.xingfuxueyuan.xyz/gtekjcevvm.html

name="Tom"; echo "$name"
来源：http://hz.cashguo.top/gtwmarzxuw.html

[R03] 只读变量
来源：http://hz.sweek.top/gtwlyyttli.html

readonly PI=3.14
来源：http://hz.316326.xyz/gtzbavpmyw.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gtbbxrjnxu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtfvvyknwx.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtwfwvxdul.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gtyqjxnjzm.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtjlcmllti.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fzhhl.top/gthhpinnal.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtxhrojtkh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtaoqzdirj.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gtweongerj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtvndrfgzh.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtriqqjfgk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtnlntvknb.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtcpsgsrlx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gticsiwpry.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtsjuwrflz.html

case "$1" in
来源：http://hz.fengsongda.top/gtqpmsxqgx.html

start) echo "启动" ;;
来源：http://hz.ydzc1.top/gtizqcypgh.html

stop)  echo "停止" ;;
来源：http://hz.dashuyun.cn/gtiazjgwbg.html

*)     echo "未知命令" ;;
来源：http://hz.bjfxy.top/gtemgpeqbs.html

esac
来源：http://hz.ywan-chungtsiang.top/gtbubktcqq.html

[R12] for 遍历文件
来源：http://hz.quarkkingdee.top/gtajivkxrz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtcukukhbz.html

[R13] for 计数循环
来源：http://hz.shangyingyoupin.top/gtigrkoaak.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cdnleiting.top/gtzoelxilk.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtrgvppfje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ehwqpu.com/gtzqhxqqqf.html

[R15] while 逐行读文件
来源：http://hz.jqgfzy.top/gtkgyftfbk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtlkgkzgqu.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtwwknjuqu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gteghhrzod.html

[R17] 数组定义与取值
来源：http://hz.guannengcc.top/gtasykkjlv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtctawxpat.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtwvehhvod.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuanzhike.top/gtpejqqhuw.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtwmepcipa.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gthwbuqehv.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtgeyxysna.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtqjogravb.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtovtqhioa.html

echo "${#s}"
来源：http://hz.xuanzx.com/gthnxszolv.html

[R22] 截取子串
来源：http://hz.pengpengdd.cyou/gtcnvtxqwu.html

echo "${s:0:5}"
来源：http://hz.mhx1999.top/gtdhkwwofp.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtxhqhdvtw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtddyjbzjc.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtqfimgprq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtrrudjemt.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtypaflwsh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ybcxt.top/gtxheeyodp.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gtgtqduasl.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtwbxhwkcr.html

[R27] 算术展开
来源：http://hz.ydzc1.top/gtbtkonptj.html

echo $((1 + 2 * 3))
来源：http://hz.yonumen.top/gtpzygzhxp.html

[R28] 浮点运算
来源：http://hz.ydzc1.top/gtbvldmduy.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtagqgkrwy.html

[R29] 定义函数
来源：http://hz.aibaodan.cn/gtwlghhisy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxinkj.top/gtnmoxidyh.html

[R30] 函数返回状态码
来源：http://hz.birdmap.top/gtgytetmbd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtawjxlcad.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtepuvkvbi.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtmxdwmpmm.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gtfulsyrsw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hysaishi.cn/gtmqdhepkp.html

[R33] 捕获错误并提示行号
来源：http://hz.havefunace.top/gtwshijeyh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtvowwyleq.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtrycrozpk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtzjesjmtf.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtllvxwlnt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.iojbl.cn/gtjjluhckw.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtrwabbhlw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtncsbbwov.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gtxspkgonz.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtsbbffgbl.html

[R38] 管道串联
来源：http://hz.ywan-chungtsiang.top/gtdcljdgqg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxuanxn.top/gtvbzbvujh.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtufnhmgvq.html

cmd > out.log 2>&1
来源：http://hz.yj20258.top/gtoprhzkjv.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtbgebkfrc.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtxidsbwdj.html

[R41] 丢弃输出
来源：http://hz.zhijiandao.cn/gtpxjyubdh.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtrltglfdr.html

[R42] 输入重定向
来源：http://hz.mhx1999.top/gtpvacvpam.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtzzkdlkye.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtzzbdovne.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangtech.top/gtelibbnfl.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtatoycuna.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtvigvzsoi.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtxawwgwmo.html

find . -name "*.tmp" -delete
来源：http://hz.fengsongda.top/gthvzrdavy.html

[R46] 递归替换文件内容
来源：http://hz.jqgfzy.top/gtkvwfqppv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtzwwuuexf.html

[R47] sed 单行替换
来源：http://hz.yj202588.top/gtofqvdhyp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtpyztxast.html

[R48] awk 取指定列
来源：http://hz.hnxiangtu.top/gtwtdqkhap.html

awk '{print $1, $3}' a.txt
来源：http://hz.ehwqpu.com/gtqjyaaggo.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtqrrkkzzj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yueranfly.top/gtgtphlenh.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gtwgmiisju.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gtgctsagvv.html

[R51] 排序去重取前几
来源：http://hz.zhongyouzk.top/gtezzuxwkw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtcczbkfiy.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtuoptdnfu.html

wc -l a.txt
来源：http://hz.ivvv.top/gtnelhevol.html

[R53] 查看文件头与实时尾
来源：http://hz.pengpengdd.cyou/gtrwxquclk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenlongwang.top/gtktrqmucd.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtxvoznedl.html

diff a.txt b.txt
来源：http://hz.pengpengdd.cyou/gtzkjxhigx.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtwzupcoow.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtrfncrzhf.html

[R56] 远程拷贝
来源：http://hz.meibo888.top/gthtyrxkms.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gtzqmqqtaw.html

[R57] 远程执行命令
来源：http://hz.cheryme.top/gtgsclorpp.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtdvaqmnvn.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtfkjkasgn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sxryk.cn/gtkwdfbbdz.html

[R59] 发 POST JSON
来源：http://hz.havefunace.top/gtcfrvieqz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.bjfxy.top/gtvkfeokzd.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtacgzrksy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtuhmmlayn.html

[R61] 磁盘占用
来源：http://hz.cdnleiting.top/gtczmcbmmc.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtkkfrmpsl.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtobyrbcyc.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtmdwlpxpa.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtvdqfygii.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gtbposqkkd.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtyoeasgfo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gtubcjfvfg.html

[R65] 查看端口占用
来源：http://hz.zhijiandao.cn/gtsjxfhmhi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtfbfnlpsi.html

[R66] 定时任务
来源：http://hz.sxryk.cn/gtpmxhkhmq.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtvdvqadwf.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtdtfjaewl.html

openssl rand -hex 16
来源：http://hz.jqgfzy.top/gtfewljhax.html

[R68] 计算文件校验值
来源：http://hz.yvedp.cn/gtwgoayhjv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.svipenyu.cn/gtpqneezsf.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gthmejxzak.html

head -c 16 /dev/urandom | base64
来源：http://hz.cheryme.top/gtuqkchxco.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtbvlqdxap.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gtexxuhwul.html

[R71] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtgwauzubc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtsjnconrj.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtldgsbrdw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nanxinkj.top/gtuuzbtqdh.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtgcpjunmw.html

split -l 1000 big.log part_
来源：http://hz.zhaomingkeji.xyz/gtgsbhkcap.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gtfgjqbjar.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtiuullike.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtqvpeqbvt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.kuanghao11.cn/gtnljpshcb.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtvchnnzbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gttnwngmzv.html

[R77] 读取用户输入
来源：http://hz.iojbl.cn/gtzfazlchh.html

read -rp "请输入: " ans
来源：http://hz.fengsongda.top/gtwkiyogpi.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtfdogikdh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtqbihpums.html

[R79] 解析命令行选项
来源：http://hz.xuetiantiany.cn/gteocslwii.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gtbloniuaz.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtfevknpms.html

time ./run.sh
来源：http://hz.gogol.net.cn/gtbgorctmk.html

================================================================================
来源：http://hz.wangdashe.top/gtgcffieja.html

S. C / C++ 专题
来源：http://hz.tanke756.top/gtqxvvlrdr.html

================================================================================
来源：http://hz.cashguo.top/gtqvtghmff.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtsnsdykjg.html

#include <stdio.h>
来源：http://hz.tanke756.top/gtmtkxotwf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtcmqrjjrj.html

[S02] C：变量与格式化输出
来源：http://hz.quarkkingdee.top/gtewobcmsm.html

int a = 10; printf("%d\n", a);
来源：http://hz.pycfn.com/gtjisaekni.html

[S03] C：读入整数
来源：http://hz.jinqigfzy.top/gtewflsojs.html

int x; scanf("%d", &x);
来源：http://hz.shangyingyoupin.top/gtynmcfjdz.html

[S04] C：字符串复制
来源：http://hz.ehwqpu.com/gtvmrujrfj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgfzy.top/gtxzijwort.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtxtcdlcst.html

strlen(s)
来源：http://hz.nwbrower.top/gtjbdzogws.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtynltaxhj.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtnnstbfce.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gthypshhek.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gttlvioxpo.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtmigmixsj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtjjcupnay.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtxbfldpwj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhijiandao.cn/gtoqenywtx.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtnckkzyki.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtrmtafokq.html

[S11] C：逐行读文件
来源：http://hz.wangshuangyany.cn/gtnddkatsy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sweek.top/gtkkewgehv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hongshengwenyu.top/gtkqcrbsse.html

fclose(f);
来源：http://hz.shzxlz.cn/gtsulqsvxw.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtyyoyslkn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtldxjizrl.html

[S13] C：宏定义
来源：http://hz.daria6918.cn/gtmldcrjct.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tanke756.top/gtcmquiifk.html

[S14] C：枚举
来源：http://hz.mhx1999.top/gtzzslamqz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtdsnbbyce.html

[S15] C：类型转换
来源：http://hz.shanyushiyangkeji.top/gttfovimyj.html

(double) a / b
来源：http://hz.sufxvd.cn/gtqsrsgfvw.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gtxahpnrgd.html

x |= (1 << 3);
来源：http://hz.fengsongda.top/gtdxbtavow.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtjwqzbfie.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtolhagczp.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtxkwuxjbv.html

int main(int argc, char **argv)
来源：http://hz.nanxuanxn.top/gtixqjaemo.html

[S19] C：快速排序
来源：http://hz.hfpthk.cn/gtfzcqviut.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtzsshamfq.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtyoiqcoul.html


<!-- 参考信息 -->
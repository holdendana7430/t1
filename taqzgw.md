代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gtepfdtlbp.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtodwncnvy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtcvdzlspn.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtejezkflg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtigppnivi.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtqyltvlxq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.feifeiyinyue.top/gtflbuotyp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtpoyfewyj.html

[Q61] 移动平均
来源：http://hz.shangyingyoupin.top/gtevvwwuuj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtrdtjagxv.html

[Q62] 分组占比
来源：http://hz.vqdsnc.cn/gtoclrmluj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtdjwcpknz.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtombievvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtaowdptwh.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtumyqcwnf.html

COMMIT;
来源：http://hz.zhaomingkeji.xyz/gtsildbvvr.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtwmvweibh.html

ROLLBACK;
来源：http://hz.ydjk.org.cn/gtqwcydmpe.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtthmpmhxf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daxiang520.top/gtooqjbwmx.html

[Q67] 设置隔离级别
来源：http://hz.xziqi.cn/gtgggmlfig.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigfzy.top/gtrrlooazt.html

[Q68] 保存点
来源：http://hz.havefunace.top/gtssfotzgo.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gtilistnpb.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtgyrvwtms.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtgrnzlyvk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.birdmap.top/gtufvlfoea.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gtolqptsxs.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtmjvqaudd.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtqyrahfay.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jiagoushi.top/gtmkhdkvhl.html

[Q72] 查看索引
来源：http://hz.jinqigufen.top/gtumleauhl.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtyjshjbvb.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtpuckoipz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cheryme.top/gteqxonrix.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gtwosndvom.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gthudfrkwr.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtddcrfpjv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtkcqhohwy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shzxlz.cn/gthvzrcvof.html

[Q76] 按天统计
来源：http://hz.xuanzx.com/gtdvqewoyz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shuidangran.top/gtuskwzlka.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtfnsvbgjk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yangfankeji.com/gtsezasrba.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtivayrcej.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.9152youxi.cn/gtmcbzjujr.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtttqqyfch.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gtprsiwlgf.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gtxvlpjybz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtndmbcvro.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtjsahxcgs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtzmthgzrz.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtwjlcukjr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenzaomai.com/gtmgqezxiw.html

[Q83] 大小写转换
来源：http://hz.xuetiantiany.cn/gtphuthzxu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtxcirjzst.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtklmuwlkd.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtdnivnmav.html

[Q85] 数值取整
来源：http://hz.vqdsnc.cn/gthkjxydgc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fengsongda.top/gtshqaksyr.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gtmerikchz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtyvuiomvk.html

[Q87] JSON 字段做条件
来源：http://hz.ppjwa.cn/gtqhnqjatj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gtczgpygae.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtlnyluvlm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtushebjlg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gtywsyzmlf.html

[Q89] 判断表是否存在
来源：http://hz.jinyuanbaomall.cn/gtrctvyfkb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.iojbl.cn/gtommghtsl.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gthorkubjx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtsouizclf.html

================================================================================
来源：http://hz.wangdashe.top/gtfyodshyt.html

R. Bash 专题
来源：http://hz.zhongyouzk.top/gtcxgpfqfi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqoimpmly.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtnziftsog.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtcquvlros.html

set -euo pipefail
来源：http://hz.zdqjudy.top/gtykexjoma.html

[R02] 变量赋值与使用
来源：http://hz.zhijiandao.cn/gtlqekgmci.html

name="Tom"; echo "$name"
来源：http://hz.shangyingyoupin.top/gtuehldwfh.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtorhdoyln.html

readonly PI=3.14
来源：http://hz.hywenlv.cn/gtrucutfte.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtgbcjadmf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtyjkiarwk.html

[R05] 参数默认值
来源：http://hz.shanyushiyangtech.top/gtxrqpihcy.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gthefahuav.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtilbqlfmm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gotoacloud.top/gtohnopmix.html

[R07] if 判断文件
来源：http://hz.svipenyu.cn/gtkbaplcvq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fzhhl.top/gttoshfvwc.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtyyhlqmjr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtqxelzoev.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtmhoxjyxh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guowangkeji.top/gtqzftlula.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtwnbeborx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258.top/gtnfvbvqhs.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtbqumgiij.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtkxzrcpfu.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtnsqmdnck.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtfgabeejz.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtmtulcrva.html

esac
来源：http://hz.quarkkingdee.top/gtmcpbabjz.html

[R12] for 遍历文件
来源：http://hz.cucudq.cn/gtbfeanifl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtpesbhqvk.html

[R13] for 计数循环
来源：http://hz.yongpay.top/gtrtacfjnx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtskrmfuue.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtpelyftwa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtgzwwieqo.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtyuwnbwrl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangkeji.top/gtwdphvgun.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtnhjvclrm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtvxxzfdmz.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtedxxxcph.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tianlin.xyz/gtpxqaueqx.html

[R18] 遍历数组
来源：http://hz.aibaodan.cn/gtrqoousps.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ppjwa.cn/gtiyigqhps.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtoyfyhszo.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gtmuchrncy.html

[R20] 关联数组（字典）
来源：http://hz.cdnleiting.top/gtifpxgbko.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gtmckklfwv.html

[R21] 字符串长度
来源：http://hz.ydzc1.top/gtzgiskprg.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtvwkhxqot.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtpkkebxce.html

echo "${s:0:5}"
来源：http://hz.haohaochexian.top/gtlwnlwcta.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtxycnrhjk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.quarkkingdee.top/gtbsvfqwzt.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gthuhxkiin.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtwkkxcago.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtinxedyta.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtjspoeqjq.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gtvivrvehh.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtqtugvhwl.html

[R27] 算术展开
来源：http://hz.jinyuanbaomall.cn/gtqqdbbcfo.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gttupppgnw.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtofwweggn.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydjk.org.cn/gtwirjlkkm.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtqewudqak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtvathpwcl.html

[R30] 函数返回状态码
来源：http://hz.svipenyu.cn/gtsmvumpmr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yvedp.cn/gtguwyniud.html

[R31] 局部变量
来源：http://hz.tanke756.top/gtlsmmeeqr.html

f() { local x=1; echo "$x"; }
来源：http://hz.hywenlv.cn/gtlynhtyug.html

[R32] 参数个数校验
来源：http://hz.tian-w.cn/gtidywrdlc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtxwhhjnoe.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtnoqphikd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtbdqpucux.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gtrgsrtnbb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtioyadaao.html

[R35] 后台执行并等待
来源：http://hz.jinyuanbaomall.cn/gtlnlwggww.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtiziahnky.html

[R36] 并发执行多个任务
来源：http://hz.ywan-chungtsiang.top/gtcaargfen.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtdfabheha.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gtpzyxhlky.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtthxzwkyj.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtwnfzyxzx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtuuhhhjbc.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtxpfvzvja.html

cmd > out.log 2>&1
来源：http://hz.daxiang520.top/gtdjkhsaxc.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtxftqqgja.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtxnrwlcqn.html

[R41] 丢弃输出
来源：http://hz.wangshuangyany.cn/gtnhnkwitn.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtnmzxjjjn.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtdhezfucp.html

wc -l < a.txt
来源：http://hz.chenlongwang.top/gtpahhaggp.html

[R43] 按名字查找文件
来源：http://hz.hammf.cn/gtnabiyxty.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtmxmcxbbe.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gttesuvoes.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtgousyqgb.html

[R45] 批量删除
来源：http://hz.bjfxy.top/gtmthwiinx.html

find . -name "*.tmp" -delete
来源：http://hz.chenzaomai.com/gthnapurle.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtiyeqxoqy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtgduipjht.html

[R47] sed 单行替换
来源：http://hz.jyoumei.cn/gttophdhvq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.kuanghao11.cn/gtugosqrvj.html

[R48] awk 取指定列
来源：http://hz.jiagoushi.top/gtkzshozll.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtjcixyckq.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gtuadmetgd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtbqrspnxq.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtopbggjtz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtydypnmxm.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gtpbnlmhhv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtltnakliu.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtplmrswbv.html

wc -l a.txt
来源：http://hz.yj20258888.top/gthsfycwla.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtfcqfscen.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.havefunace.top/gtbombziii.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gthaijefes.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtgswhyxpx.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gtpnfjnowl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtyevkiqvg.html

[R56] 远程拷贝
来源：http://hz.gaohongyu789.top/gtpawvwncg.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtgpdnaqam.html

[R57] 远程执行命令
来源：http://hz.hnxiangtu.top/gtdibmzayr.html

ssh user@host 'uptime'
来源：http://hz.havefunace.top/gtfufgkkjz.html

[R58] 下载文件
来源：http://hz.cdnleiting.top/gtbomrgpjl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtilmazmja.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtobsurnig.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xinyue.icu/gttiztdmls.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gtkopkgfzb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtnqimbada.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtyavvhofr.html

df -h;  du -sh *
来源：http://hz.zhongyouzk.top/gtmzelldfm.html

[R62] 找最占空间的文件
来源：http://hz.ivvv.top/gtdipqurql.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258888.top/gthwdtgzxw.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gttnuahqad.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtspcdgtia.html

[R64] 结束进程
来源：http://hz.feifeiyinyue.top/gtrppirysi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gtfzkjzbym.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtioiiyedn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gtmiydhvve.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gtztbdzjfh.html

crontab -e;  crontab -l
来源：http://hz.yonumen.top/gtgckrwcfr.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtrndmpohu.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtwcjwmsak.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtusbvupra.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtfouvtrkr.html

[R69] 生成随机密码
来源：http://hz.chenjidiqi.icu/gtpzegawfx.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtnfbsruaj.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gtuhhtmevi.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtaxltswdi.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtadxzianf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj202588.top/gtokxhtfwm.html

[R72] 等待端口就绪
来源：http://hz.xuanzx.com/gtoampwles.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuanzx.com/gtvezwirsj.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gtrzjjhvow.html

split -l 1000 big.log part_
来源：http://hz.zhengqikj.top/gtrqiyklkc.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gtmacqkorp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gttrytgbkl.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtiwltibeu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtjdelaeft.html

[R76] 使用临时文件
来源：http://hz.smart0.xyz/gtjzwdsdwt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtdoftyxpy.html

[R77] 读取用户输入
来源：http://hz.svipenyu.cn/gtyskesahg.html

read -rp "请输入: " ans
来源：http://hz.jqgufenzy.top/gtunqjuzyz.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtmrxkoqpz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gttfraqvkd.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtegxseoox.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtcettvasc.html

[R80] 查看脚本执行耗时
来源：http://hz.jlsjyb.cn/gtkovxdrwj.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtvebkeszq.html

================================================================================
来源：http://hz.shzxlz.cn/gtiqziciev.html

S. C / C++ 专题
来源：http://hz.gogol.net.cn/gtpzleqfzu.html

================================================================================
来源：http://hz.cucudq.cn/gtxzywauvu.html

[S01] C：Hello World
来源：http://hz.chenlongwang.top/gtgurhgrpf.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gthtqxbbgp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yonumen.top/gtfzbsosux.html

[S02] C：变量与格式化输出
来源：http://hz.jqgfzy.top/gtjfyqifaf.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtdzpzscrn.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtilrkujnu.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gtndvfusso.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtawjbszfi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuanzhike.top/gtjfumvjrg.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtebpglbky.html

strlen(s)
来源：http://hz.sufxvd.cn/gtivzqvhxq.html

[S06] C：字符串比较
来源：http://hz.ivvv.top/gtkuybhkpz.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtqouaerhb.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gtphqdchru.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daria6918.cn/gtdndoclnv.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtodvuonqy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtebpilfcg.html

[S09] C：结构体定义与初始化
来源：http://hz.cashguo.top/gtiknthnof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gotoacloud.top/gtsxdjelvx.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtcoienqqa.html

int *p = &a;  *p = 5;
来源：http://hz.ywan-chungtsiang.top/gtgsiavkyk.html

[S11] C：逐行读文件
来源：http://hz.fengsongda.top/gtprcxqewz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gttnfqoxhg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhongyouzk.top/gttzznwsgu.html

fclose(f);
来源：http://hz.yuanzhike.top/gtprhwjjvh.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gtxxyvongm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtjpmtnivh.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtayslobjb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gtlopsaape.html

[S14] C：枚举
来源：http://hz.kuanghao11.cn/gtyxxppdws.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtpqcdhaiz.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtuceqeahz.html

(double) a / b
来源：http://hz.jqgfzy.top/gtftximjzg.html

[S16] C：位操作置位
来源：http://hz.hysaishi.cn/gtutwdaoka.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtojkubidn.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gtiwfypspp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aibaodan.cn/gtoxvimbhh.html

[S18] C：命令行参数
来源：http://hz.cqqwz.cn/gtvfkxmmhz.html

int main(int argc, char **argv)
来源：http://hz.zhijiandao.cn/gtidpjuzua.html

[S19] C：快速排序
来源：http://hz.zhixingplan.top/gtuiegtlpg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gttxprdmdg.html

[S20] C：二分查找
来源：http://hz.xylfe.cn/gtwcckdbkh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtmfvkfhqd.html

[S21] C：字符类别判断
来源：http://hz.sxryk.cn/gtagarkade.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pycfn.com/gtttvvffyk.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtvvwlttlo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtdetfovut.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtdzupcurr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhijiandao.cn/gtfmlmbrou.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gtspwassre.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigufen.top/gtahqkngoy.html

[S25] C：内存拷贝
来源：http://hz.hammf.cn/gtzyrlzswz.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtahtpoqaa.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gthictfizz.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtcbtbnqcq.html

[S27] C：定义常量
来源：http://hz.birdmap.top/gteiqhaknq.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtgawdqpvo.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtzhknoozm.html


<!-- 参考信息 -->
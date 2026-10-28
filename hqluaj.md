代发 wailian999

[Q65] 回滚事务
来源：http://hz.shzxlz.cn/gtrhutwsnu.html

ROLLBACK;
来源：http://hz.bjfxy.top/gtvybejcch.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtuixfpopm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guannengcc.top/gtndiltruf.html

[Q67] 设置隔离级别
来源：http://hz.fzhhl.top/gtjpaahbhj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtbqkghovq.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gthfbtimxf.html

SAVEPOINT sp1;
来源：http://hz.guannengcc.top/gtimijjcev.html

ROLLBACK TO sp1;
来源：http://hz.xylfe.cn/gtiozhyhsr.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gtswligybt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtxvdxqyge.html

[Q70] 更新统计信息
来源：http://hz.zhiwuduotai.top/gtocvcujau.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtjgsmmsxv.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtktrwzeuj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtkfigvwrv.html

[Q72] 查看索引
来源：http://hz.guowangkeji.top/gtnvljvsya.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gtlalkhyfw.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtwtauvylo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtuksbgdhy.html

[Q74] 强制使用索引
来源：http://hz.wangdashe.top/gtymfzueox.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aibaodan.cn/gtdcmojlcy.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gtbslxkfdz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtipbefymr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhoulong.xyz/gtcmyrfakd.html

[Q76] 按天统计
来源：http://hz.svipenyu.cn/gtayhvawjl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fengsongda.top/gtyxjnmzbl.html

[Q77] 时间加减
来源：http://hz.svipenyu.cn/gtpwkgjvqy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gttzuucxmi.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtfmetadhr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gtytogfkxp.html

[Q79] 字符串拼接
来源：http://hz.jqgfzy.top/gtpszqwafc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.9152youxi.cn/gtzallerpw.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gtwtycmgjx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtilrhzgva.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtcbuorsxi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.andypj.xyz/gttvhmhusd.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtkdypjlbv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtjtvyrltf.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtizclyhyh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtplyaijzd.html

[Q84] 去除首尾空格
来源：http://hz.cucudq.cn/gtjpgclffa.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtwdhqrzmf.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtydxssxfe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtbxfuoarv.html

[Q86] 读取 JSON 字段
来源：http://hz.bjfxy.top/gttnbpvnan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gthwmthpmt.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtgennqyts.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pengpengdd.cyou/gtxxqidfzh.html

[Q88] 行转列（条件聚合）
来源：http://hz.snrcjt.cn/gtzvejeamr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtxxnoucvc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jyoumei.cn/gtrbtzhrtg.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtpkfymyis.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtvpihhzzw.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtibbrfdrr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.quarkkingdee.top/gtdlbulpyu.html

================================================================================
来源：http://hz.tanke756.top/gtvlvczudr.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtymygxbix.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnnvqptvq.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gtwaopfhdz.html

#!/usr/bin/env bash
来源：http://hz.xziqi.cn/gtwibcfbpa.html

set -euo pipefail
来源：http://hz.yj20258.top/gtzethords.html

[R02] 变量赋值与使用
来源：http://hz.hywenlv.cn/gtytsnbqmi.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtzmpxpyhm.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtotnzofta.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtjqdxzcaj.html

[R04] 位置参数
来源：http://hz.fzhhl.top/gtuvhdzass.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtnayiwiay.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gthebjzopu.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtyxamvfxo.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtgbrvkvyh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hywenlv.cn/gthwrvfsgd.html

[R07] if 判断文件
来源：http://hz.chenlongwang.top/gtigrykjvr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gtwwuzpmlz.html

[R08] 数值比较
来源：http://hz.316326.xyz/gteupbvvyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gogol.net.cn/gtwhowtyxv.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gtcqagpbgp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258888.top/gtaedenceq.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtcapjeebt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.quarkkingdee.top/gtdpfcgadn.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtunnvtqrd.html

case "$1" in
来源：http://hz.sufxvd.cn/gtentkmuzf.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtvyebsbiu.html

stop)  echo "停止" ;;
来源：http://hz.316326.xyz/gtidayrxmz.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gteujiijud.html

esac
来源：http://hz.bjfxy.top/gtslcbtjtr.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtalokmxgj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jiagoushi.top/gtwbrjdvnp.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtyisjcwzq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dashuyun.cn/gtuqqrxytp.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gtsgukttzj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtepudhvpq.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gtjikgkooz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtafcrkraj.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtnvdodkqw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtzddfpkxo.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtkymdvaom.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtulibflyh.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtwfmvcnop.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gtiqdozfau.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtsxojsjqc.html

echo "${#arr[@]}"
来源：http://hz.haohaochexian.top/gttnzgyccq.html

[R20] 关联数组（字典）
来源：http://hz.xinyue.icu/gthbwcrmdw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtystbpyvs.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gtmtnohpin.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtbtwtfsmx.html

[R22] 截取子串
来源：http://hz.cucudq.cn/gttzkdpwky.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtsfnibmpv.html

[R23] 字符串替换
来源：http://hz.hnxiangtu.top/gtuhlncbxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gtctvhfnvf.html

[R24] 大小写转换
来源：http://hz.yongpay.top/gtuddkkpbr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtuoayhcml.html

[R25] 去后缀 / 去前缀
来源：http://hz.guannengcc.top/gtdflsnxws.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtmpxrdbyh.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtcndlypyu.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtxlzwvhee.html

[R27] 算术展开
来源：http://hz.sxryk.cn/gtgzzbykmc.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtgxcetmlb.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtsodznwcp.html

echo "scale=2; 10/3" | bc
来源：http://hz.tanke756.top/gtjinodtjv.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtchgvevkl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtocnuhwkj.html

[R30] 函数返回状态码
来源：http://hz.dashuyun.cn/gtcgozrinj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xziqi.cn/gtadxbxdfy.html

[R31] 局部变量
来源：http://hz.ywan-chungtsiang.top/gtnaahjsoq.html

f() { local x=1; echo "$x"; }
来源：http://hz.yanxiufei.cn/gtfowdemke.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtrtcwfckh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtdmtejfhm.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtfmtncmyp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtbalfudul.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtepwlpbgi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtjsbldzot.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtweetbzka.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gtobdjrpvv.html

[R36] 并发执行多个任务
来源：http://hz.zhongyouzk.top/gtvprbnfpb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtfojmpzyp.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gtzlwxhzde.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gtoyvcflae.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtweolfomp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtpuxqhjqn.html

[R39] 重定向标准输出与错误
来源：http://hz.jlsjyb.cn/gtvxqacwuu.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtomkvxpbq.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtieygseog.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtfkatutpb.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtpazwremw.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtllwyyuuo.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtosoyclii.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtxmpaqmin.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtuhybmvrl.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtmbvrgacr.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtbqzkskmm.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtucajbilw.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtdvrlepoa.html

find . -name "*.tmp" -delete
来源：http://hz.zhijiandao.cn/gtadiuxjrn.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtlfagzywp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtjpbvyiaf.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gteblxnzuo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtpnaekykt.html

[R48] awk 取指定列
来源：http://hz.zhiwuduotai.top/gtgvvvphno.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtjhmbsthx.html

[R49] awk 带条件
来源：http://hz.yj20258888.top/gtwjodrulr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuetiantiany.cn/gtbhysensr.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gtoospnzxb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gttzzocxcn.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtodvhliap.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtuwqibzfv.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtzrkmfrke.html

wc -l a.txt
来源：http://hz.sysykeji.top/gtkdiihrif.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtpwiffuvd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.9152youxi.cn/gtbmmygubm.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gtqlgixtzy.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gthzoyjell.html

[R55] 压缩与解压
来源：http://hz.cucudq.cn/gtynpwupdn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtqececjvv.html

[R56] 远程拷贝
来源：http://hz.gaohongyu789.top/gthmribfxm.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtnawehwzb.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtjtoiwmnr.html

ssh user@host 'uptime'
来源：http://hz.jinyuanbaomall.cn/gtwlierpll.html

[R58] 下载文件
来源：http://hz.nanxinkj.top/gtgfsuhnfd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtxgfvpbby.html

[R59] 发 POST JSON
来源：http://hz.jyoumei.cn/gtsdcsykpj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtugfnltqd.html

[R60] 只看 HTTP 状态码
来源：http://hz.ybcxt.top/gtvymfghdb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtcorpjkru.html

[R61] 磁盘占用
来源：http://hz.cheryme.top/gtvtpshrou.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtbccqznhu.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gtgyfegqmk.html

du -ah . | sort -rh | head -10
来源：http://hz.sweek.top/gtbmdrdvob.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtscwqdath.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtkjpyduxo.html

[R64] 结束进程
来源：http://hz.yueranfly.top/gtsqxmzcyp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nanxinkj.top/gtkvbvilnh.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtwyqzhmax.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hysaishi.cn/gtjusjgxij.html

[R66] 定时任务
来源：http://hz.yj20258888.top/gtkfijrjva.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtreiqrbap.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtutkcwtzd.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtlhyjslzs.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gtdyswhxly.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtkrqtwxqi.html

[R69] 生成随机密码
来源：http://hz.0kj1m.cn/gtoyzpaews.html

head -c 16 /dev/urandom | base64
来源：http://hz.ywan-chungtsiang.top/gthcbkntuh.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtdspiunva.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtoqbjsaah.html

[R71] 日期格式化
来源：http://hz.shzxlz.cn/gtsvassmsp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gthckqulmy.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtiflmqqsz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtvjfjimfm.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtcvjaxmcz.html

split -l 1000 big.log part_
来源：http://hz.tian-w.cn/gtfdqnbjsm.html

[R74] 批量重命名
来源：http://hz.xziqi.cn/gtqtdwejwk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtmrzuwalr.html

[R75] 导出环境变量
来源：http://hz.xuanzx.com/gtrgplukjs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtjdoopnlo.html

[R76] 使用临时文件
来源：http://hz.andypj.xyz/gtndqpjsrh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtcjpjvmve.html

[R77] 读取用户输入
来源：http://hz.ydjk.org.cn/gtmxhfqgae.html

read -rp "请输入: " ans
来源：http://hz.smart0.xyz/gtvhbyhvep.html

[R78] 交互式菜单
来源：http://hz.c1oappe.top/gtzjxgwdft.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gttvxyebuv.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtvrqxspip.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xylfe.cn/gtjosdnqcp.html

[R80] 查看脚本执行耗时
来源：http://hz.jinyuanbaomall.cn/gtyfdhemjm.html

time ./run.sh
来源：http://hz.zdqjudy.top/gtuebioapb.html

================================================================================
来源：http://hz.sxryk.cn/gtemdoyyqm.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtoyphjhsb.html

================================================================================
来源：http://hz.yuanzhike.top/gtighfjbhp.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gtyzxaekuv.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtcywgavlf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtqpbbzheh.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtheokmuef.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangdashe.top/gtgpwvbldb.html

[S03] C：读入整数
来源：http://hz.yj20258888.top/gtbltjpntc.html

int x; scanf("%d", &x);
来源：http://hz.9152youxi.cn/gtgaqvsthy.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtaztxszir.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj202588.top/gtbtzckibw.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gtcnvrkwcy.html

strlen(s)
来源：http://hz.gogol.net.cn/gtdhxnaslq.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gttfhownvz.html

strcmp(a, b) == 0
来源：http://hz.cashguo.top/gtmmaejxzi.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtoryzlogh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtbqygqadp.html

[S08] C：动态内存分配与释放
来源：http://hz.nwbrower.top/gtyslkzswj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtacbdwwmz.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gtymqzysyr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yangfankeji.com/gtoszieoay.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtjzdeadxw.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtucyajcdb.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gtcosqzrnj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtmclnmhit.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gtvvobzfep.html

fclose(f);
来源：http://hz.jqgfzy.top/gtkzeqwsnu.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtzxehxzmp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhijiandao.cn/gtdjdwywjt.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtjutkmkyq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuanzx.com/gtbogdmxku.html

[S14] C：枚举
来源：http://hz.ydjk.org.cn/gtpfiscjis.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtihtzlvmv.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtzncaqrev.html

(double) a / b
来源：http://hz.dianchejie.cn/gtjnqqsgzl.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gtqeoswhup.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtbkprnffi.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtfourrwhq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yongpay.top/gtnfdrpezx.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtfegicnua.html

int main(int argc, char **argv)
来源：http://hz.zhaomingkeji.xyz/gtilrgquek.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtxovloepj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtqimzrmhw.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtpitvxwca.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gttakrvssw.html

[S21] C：字符类别判断
来源：http://hz.hywenlv.cn/gtqctasjud.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.smart0.xyz/gthcmuhgsq.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtbdgrwauz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cashguo.top/gtvlbjcouj.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtkymbovuu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtvrtulguw.html

[S24] C：获取本地时间
来源：http://hz.tianlin.xyz/gtwmiwvgnb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gtxyrfuxsa.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtuifyrgfq.html

memcpy(dst, src, n);
来源：http://hz.dashuyun.cn/gtespaikmu.html

[S26] C：内存清零
来源：http://hz.meibo888.top/gtljbugqph.html

memset(a, 0, sizeof a);
来源：http://hz.316326.xyz/gtxpfwkkms.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtsvdnsibx.html

const double PI = 3.14159;
来源：http://hz.cdnleiting.top/gtoatiygxp.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gttycytgpq.html

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gtabuzxfzo.html

[S29] C：变参函数
来源：http://hz.sufxvd.cn/gttwjcldrj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtubogzbxo.html

[S30] C：头文件保护
来源：http://hz.cucudq.cn/gtihcflxkd.html

#ifndef X_H
来源：http://hz.jqgufenzy.top/gtmnysyztj.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtqepwtrts.html

#endif
来源：http://hz.tianlin.xyz/gthaspsnri.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtwmfcdend.html

#include <iostream>
来源：http://hz.cashguo.top/gtefzlzcqa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtnjgigwpw.html

[S32] C++：字符串
来源：http://hz.cheryme.top/gtkvxefzck.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gtbkqtdlph.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtlfymvnut.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtriecchkz.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gtyashbyxl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtxtpczwcv.html


<!-- 参考信息 -->
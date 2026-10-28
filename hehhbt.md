代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtroceiido.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gtkaapybpb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gttgcwqwrw.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtlvpqpowf.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtsmxqnkeu.html

[Q71] 查看建表语句
来源：http://hz.chenjidiqi.icu/gtkwfhdrjl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gtmfmyfkjh.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtomupwlrx.html

SHOW INDEX FROM users;
来源：http://hz.guowangkeji.top/gtnrmmvlrb.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gtamelofic.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cqqwz.cn/gtrgqoxtqe.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtogdmdiuh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtnmdmzqhm.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtinqcrquz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aibaodan.cn/gtgwflnurw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtjitnptvh.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gtjqvadtgn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtsdveqidr.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gtzsmfqygy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtyfgwamyg.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gthfenpusf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtssdqvbxa.html

[Q79] 字符串拼接
来源：http://hz.chenzaomai.com/gtaasedzzw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtysikakor.html

[Q80] 字符串截取
来源：http://hz.gzhubu.top/gtenyfhtga.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dashuyun.cn/gttmkutftc.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gtuqcmbhkz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gttxbugpyy.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtxeacncsx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuanzx.com/gthbsdwiyn.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtdiiemtnh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guannengcc.top/gtymtynfwb.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtbzaxfsbk.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuanzx.com/gtqaarypkn.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtcyciolck.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gtoipcnvdy.html

[Q86] 读取 JSON 字段
来源：http://hz.jinyuanbaomall.cn/gtbmmegvhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtybegrwtr.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gteatyoypn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtxvgasalj.html

[Q88] 行转列（条件聚合）
来源：http://hz.jianghu66.top/gtmgwanibi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtvolxbuuk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.redwolf501.top/gthlkrongv.html

[Q89] 判断表是否存在
来源：http://hz.gaohongyu789.top/gtbexdkilr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtkvzdamez.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtitltebin.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtjzphrfag.html

================================================================================
来源：http://hz.wangdashe.top/gtiusqbpdf.html

R. Bash 专题
来源：http://hz.zhoulong.xyz/gtmoyoopme.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtexsskshq.html

[R01] shebang 与严格模式
来源：http://hz.hammf.cn/gtapowrovr.html

#!/usr/bin/env bash
来源：http://hz.yuxming.cn/gtjfswocns.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gtaijmyjtd.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtsbfzhhwe.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtjbdiipcd.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtfdoqqlvy.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtmmiqmtvx.html

[R04] 位置参数
来源：http://hz.bjfxy.top/gtbcuyamjy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydjk.org.cn/gtvefeiofj.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtrlsxnfge.html

name="${1:-default}"
来源：http://hz.0kj1m.cn/gtswriilxs.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtkqtbtdhj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtfvpphcth.html

[R07] if 判断文件
来源：http://hz.shuidangran.top/gtmnwixlpi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yvedp.cn/gtdoqmydqs.html

[R08] 数值比较
来源：http://hz.fzhhl.top/gtksupnamc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ybcxt.top/gttwuxthne.html

[R09] 字符串比较
来源：http://hz.snrcjt.cn/gtkgmfsein.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.svipenyu.cn/gtpuojjgab.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtirdxsmir.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gttdetkcru.html

[R11] case 多分支
来源：http://hz.gogol.net.cn/gtfwxkcrff.html

case "$1" in
来源：http://hz.andypj.xyz/gtcgxckwzi.html

start) echo "启动" ;;
来源：http://hz.zhengqikj.top/gtjabhzqhx.html

stop)  echo "停止" ;;
来源：http://hz.cqqwz.cn/gtjyjqsiun.html

*)     echo "未知命令" ;;
来源：http://hz.jinyuanbaomall.cn/gtfxmstneh.html

esac
来源：http://hz.fzhhl.top/gtjblnfbas.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtabfhyogg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gogol.net.cn/gtxefwuguk.html

[R13] for 计数循环
来源：http://hz.jqgufenzy.top/gtuersvyvz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtkznelcgf.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtrjvwivqp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yueranfly.top/gtismxkngf.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtermdaoog.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gthzdmgayh.html

[R16] until 等待条件
来源：http://hz.zdqjudy.top/gtamlclsef.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtognifdiq.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtvfsyycrr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtbkjruvoo.html

[R18] 遍历数组
来源：http://hz.hnxiangtu.top/gtwbkpgmgs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtknexzoqe.html

[R19] 数组长度
来源：http://hz.shzxlz.cn/gtsuzjatgf.html

echo "${#arr[@]}"
来源：http://hz.guannengcc.top/gtxhyjnhrt.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtkubbyoaw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guannengcc.top/gtofhdracj.html

[R21] 字符串长度
来源：http://hz.kuanghao11.cn/gtfcburppo.html

echo "${#s}"
来源：http://hz.yueranfly.top/gtterqfomn.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtqueqegkb.html

echo "${s:0:5}"
来源：http://hz.jiagoushi.top/gtvnqwkzeb.html

[R23] 字符串替换
来源：http://hz.meibo888.top/gtgxkgeivr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cdnleiting.top/gtduzutruf.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gteypdsfec.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gtzrvtghbh.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtyxrgpfaw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtncmfozra.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtgnwskckw.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtskodnmpn.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtkcjkfeyh.html

echo $((1 + 2 * 3))
来源：http://hz.xuanzx.com/gtkwyuzyqs.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtgpqutkyv.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtxxdjkywp.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtgbenjarj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtoortydgb.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gtlgcehbxa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtugdyrgxf.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gthvalwdck.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtuwpslpqb.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtengzbslt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtgqmjffwt.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtbovqycgi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtpvgfukjw.html

[R34] 退出时清理
来源：http://hz.zhijiandao.cn/gtajfttvqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtsgduvxqh.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gtqwavypol.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtqpdgtyyr.html

[R36] 并发执行多个任务
来源：http://hz.yueranfly.top/gtpiybmrjy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtdivudqwb.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtvxbnahyk.html

files=$(ls -1)
来源：http://hz.yj20258888.top/gtdiemxjti.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtuxbmwslr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guannengcc.top/gtpfmsrinz.html

[R39] 重定向标准输出与错误
来源：http://hz.jlsjyb.cn/gtekquqfaq.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtpfteaupt.html

[R40] 追加写日志
来源：http://hz.pengpengdd.cyou/gtbswmzplf.html

echo "log" >> out.log
来源：http://hz.nanxuanxn.top/gtobiopuen.html

[R41] 丢弃输出
来源：http://hz.cheryme.top/gtadqqcsrw.html

cmd >/dev/null 2>&1
来源：http://hz.jinyuanbaomall.cn/gtoxenovmx.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gtowckmgve.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtmujwzabk.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtznxcemxm.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtmpczgvoi.html

[R44] 按修改时间查找
来源：http://hz.jlsjyb.cn/gtgzaanmjb.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtaqhycmis.html

[R45] 批量删除
来源：http://hz.yj20258.top/gtlyvzozxs.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtzoedzkms.html

[R46] 递归替换文件内容
来源：http://hz.birdmap.top/gteimkawga.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuetiantiany.cn/gttyzfpvfs.html

[R47] sed 单行替换
来源：http://hz.aizwys.cn/gtfwwoqrmp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.redwolf501.top/gtoeiislzo.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtcubbjoon.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhongyouzk.top/gtqvfewigm.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtyiwrjlbi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.smart0.xyz/gthkgdubta.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtunpyxeve.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jlsjyb.cn/gtosfvfkhp.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtjbegfekj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtfipydfjr.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gtjcvoxehf.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtdfymewyv.html

[R53] 查看文件头与实时尾
来源：http://hz.shzxlz.cn/gtcigippqm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gtlaimzsow.html

[R54] 比较两个文件
来源：http://hz.zhiwuduotai.top/gtbegudmyn.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtkocxxnrk.html

[R55] 压缩与解压
来源：http://hz.xinyue.icu/gthlzlgqry.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydzc1.top/gtofczsjzp.html

[R56] 远程拷贝
来源：http://hz.gzhubu.top/gtkppksscb.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtptheebnp.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtipgnbfou.html

ssh user@host 'uptime'
来源：http://hz.nanxuanxn.top/gtvzfpmhai.html

[R58] 下载文件
来源：http://hz.jinghuilouyu.cn/gtdtnzfckp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtalhmlguz.html

[R59] 发 POST JSON
来源：http://hz.jqgufenzy.top/gtdqlvfqys.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gtqwurcrnq.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtzbwlxwzq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtvivgaplp.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtlxopsjqr.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtwaodpdhr.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtuclnfvbq.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gtcbrxwrpw.html

[R63] 内存与进程
来源：http://hz.kuanghao11.cn/gtzcmklyqg.html

free -h;  ps aux | grep nginx
来源：http://hz.xingfuxueyuan.xyz/gthyzdjpia.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtskihiuqm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtxvyukkbb.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtfwaigmmm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtgkirdupg.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtfocmyyeq.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtmqdjxpxt.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gtwgjpbsct.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gttzcdtjsy.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtyjkdnlmw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtkwrvghvg.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtacbeidsg.html

head -c 16 /dev/urandom | base64
来源：http://hz.316326.xyz/gtjdcxuvxc.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gthylcfcre.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtburaalps.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtyrxjgzxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigufen.top/gtijgjkrpm.html

[R72] 等待端口就绪
来源：http://hz.xinyue.icu/gtzdlzugwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtpsskqukw.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtwmieauyf.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gtfktgjsrf.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtavkmqljr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtmsbbfjpq.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtsmgzmxbz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zdqjudy.top/gtimlfezvl.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gtsbppvdhc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtaugkhrin.html

[R77] 读取用户输入
来源：http://hz.ivvv.top/gtgjmxwpnm.html

read -rp "请输入: " ans
来源：http://hz.nwbrower.top/gtzwtqydvc.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gticnwtoyp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hysaishi.cn/gtkkllhucg.html

[R79] 解析命令行选项
来源：http://hz.hammf.cn/gtlyszgqav.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtfbjtqmqd.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtrozksvkl.html

time ./run.sh
来源：http://hz.jianghu66.top/gtxtnxexzb.html

================================================================================
来源：http://hz.hfpthk.cn/gtkmtsmljv.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtvqjfvcqv.html

================================================================================
来源：http://hz.iojbl.cn/gtrxvrjdam.html

[S01] C：Hello World
来源：http://hz.nanxuanxn.top/gtxhsuqfjs.html

#include <stdio.h>
来源：http://hz.chenzaomai.com/gteehooczu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aibaodan.cn/gtglvvnguv.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtetfezmnf.html

int a = 10; printf("%d\n", a);
来源：http://hz.cqqwz.cn/gtvgxlaxko.html

[S03] C：读入整数
来源：http://hz.nwbrower.top/gtoakfphxa.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtjajbhqoe.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtqirhojsd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtfadeksdt.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtinoqzwzm.html

strlen(s)
来源：http://hz.sufxvd.cn/gtanadqhqj.html

[S06] C：字符串比较
来源：http://hz.0kj1m.cn/gthzsjludk.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtuhnyzutn.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtxapmtcgf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gtmsxsnxzb.html

[S08] C：动态内存分配与释放
来源：http://hz.snrcjt.cn/gtdinwmsla.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xingfuxueyuan.xyz/gtopwzfdhw.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtgfwkvntw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daria6918.cn/gtkrxzbdxu.html

[S10] C：指针与解引用
来源：http://hz.smart0.xyz/gtbudpgfji.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtdxhvdlip.html

[S11] C：逐行读文件
来源：http://hz.sufxvd.cn/gtlcjhilqc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shuidangran.top/gthcgouznd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtcnyalgrd.html

fclose(f);
来源：http://hz.zycfv.cn/gtxirolgpu.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtsccgswbh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhijiandao.cn/gtzlvowbge.html

[S13] C：宏定义
来源：http://hz.sxryk.cn/gttvmlhoic.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtyyntjfkg.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtrfngvxec.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gtdjzrwpcj.html

[S15] C：类型转换
来源：http://hz.yvedp.cn/gtqjfnndjv.html

(double) a / b
来源：http://hz.ybcxt.top/gtzbmqrwhd.html

[S16] C：位操作置位
来源：http://hz.chenlongwang.top/gtsnyunawb.html

x |= (1 << 3);
来源：http://hz.yongpay.top/gtbhfkdfop.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtohtobgut.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daxiang520.top/gtwswnrcva.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtocwvxlxq.html

int main(int argc, char **argv)
来源：http://hz.52xcode.cn/gtpleggaqc.html

[S19] C：快速排序
来源：http://hz.cheryme.top/gtfnmysvrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtehdtodoy.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtibxnaxpk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xylfe.cn/gtfrnhphex.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtonscjmhx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shangyingyoupin.top/gtxhcmzyph.html

[S22] C：字符串转数字
来源：http://hz.316326.xyz/gteudhoror.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgufenzy.top/gtddyrpjzy.html

[S23] C：随机数
来源：http://hz.sweek.top/gtjbtduzfr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gtgvkiicug.html

[S24] C：获取本地时间
来源：http://hz.jqgfzy.top/gtdarxkbaj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gttsutoetd.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gtoqdgbhlu.html

memcpy(dst, src, n);
来源：http://hz.nwbrower.top/gtffgpngtn.html

[S26] C：内存清零
来源：http://hz.hnqzz.top/gtpaczqaan.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtrfxdywgr.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtqricytli.html

const double PI = 3.14159;
来源：http://hz.ivvv.top/gtiosqipgq.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtlgdttuvb.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtklmjzlqu.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtdhaptnlv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtexcnsnvd.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtiqhdjbws.html

#ifndef X_H
来源：http://hz.daxiang520.top/gtfhdhsqah.html

#define X_H
来源：http://hz.tianlin.xyz/gtdimqowda.html

#endif
来源：http://hz.xylfe.cn/gtdivnrwlr.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtzuljdjpb.html

#include <iostream>
来源：http://hz.shuidangran.top/gtmhovbzbs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xylfe.cn/gtaqbavidk.html

[S32] C++：字符串
来源：http://hz.zycfv.cn/gtfyrptmcz.html

std::string s = "hi";  s += "!";
来源：http://hz.chenjidiqi.icu/gtcuwmvbnl.html

[S33] C++：vector 增删
来源：http://hz.yonumen.top/gtxqndeafq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtuzbtyohp.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtudymnvaw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtwnxaywnd.html

[S35] C++：map
来源：http://hz.zhiwuduotai.top/gtmwihpajc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtljhzjkfb.html

[S36] C++：unordered_map
来源：http://hz.fengsongda.top/gtwnndywkg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daria6918.cn/gtkopxrdsr.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtidphadog.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhiwuduotai.top/gtgptswiex.html

[S38] C++：排序
来源：http://hz.quarkkingdee.top/gttgnwlpbn.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtrtwrudxw.html


<!-- 参考信息 -->